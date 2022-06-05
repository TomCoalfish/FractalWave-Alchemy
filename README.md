# FractalWave-Synthesis
Synthesize fractal waves with DFT

# Theories
* https://www.synthtopia.com/content/2021/03/13/sound-synthesis-with-fractals/
* https://www.academia.edu/49846523/Fractal_additive_synthesis
* https://www.academia.edu/14589939/A_Fractal_and_Wavelet_Based_Approach_for_Audio_Coding

<image src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Flh3.googleusercontent.com%2FPWFSe9h_hpyotvvOA4FDiDIYKJBxp6xay7hKTgpeilBhHqjWTxrn5Pk0fLVKbFDa3LeVTdEt7tCkC-bt_ziHUTFfZaMHS-P8KImDchw76DKEkcRfpkXxhf03iHHqWjHUXvo&f=1&nofb=1"></image>
# Fractal Equations
* http://www.fractalsciencekit.com/program/maneqn.htm
* z = z^3 - 3*K^2*z + c
* z = z - (z^3-c)/(3*z^2)
<pre>
1--F(Z) = Z^2 + C

2--F(Z) = Z^3 + C

3--F(Z) = (Z^2 + C) / (Z - C)

4--F(Z) = Z^2 - Z + C

5--F(Z) = Z^3 - Z^2 + Z + C

6--F(Z) = (1 + C)Z - CZ^2

7--F(Z) = Z^3 / (1 + CZ^2)

8--F(Z) = (Z - 1)(Z + .5)(Z^2 - 1) + C

9--F(Z) = (Z^2 + 1 + C) / (Z^2 - 1 - C)

10--F(Z) = Z^1.5 + C

11--F(Z) = exp(Z)-C

12--F(Z) = Z - 1 + Cexp(-Z)

13--F(Z) = CZ - 1 + Cexp(-Z)

14--F(Z) = (4Z^5 + C)/5Z^4

15--F(Z) = (6Z^7 + C)/7Z^6

16--F(Z) = Z^2 * exp(-Z) + C

17--F(Z) = Z^2 * Z^(-2) + C

18--F(Z) = Z * exp(-Z) + C

19--F(Z) = C * exp(-Z) + Z^2

20--F(Z) = Z^3 + Z + C

21--F(Z) = Z^4 + Z + C

22--F(Z) = Z^4 + CZ^2 + C

23--F(Z) = Z^2sin(Re Z) + CZcos(Im Z) + C

24--F(Z) = 2^Z * CZ^2

25--F(Z) = Z^5 - Z^3 + Z + C

26--F(Z) = (Z^2 + C)^2 + Z + C

27--F(Z) = (Z + sin(Z))^2 + C

28--F(Z) = Cexp(Z)

29--F(Z) = Z^2 + C^3

30--F(Z) = Cexp(CZ)

31--F(Z) = Z^2cos(ReZ)+CZsin(ImZ)+C

32--F(Z) = CZ^2 + ZC^2

33--F(Z) = exp(cos(CZ))

34--F(Z) =(1 + Jo(Re Z))^2 + (Jo(Im Z) + C)^2 (Here Jo represents the Bessel function)

35--F(Z) = C(sin Z + cos Z)

36--F(Z) = Z^(-.5) + C

37--F(Z) = CZ(1 - Z)

38--F(Z) = C^2Z(1 - Z)

39--F(Z) = ((Z^2+C)^2)/(Z-C)

40--F(Z) = (Z + sin Z)^2 + Z^-.5 + C

41--F(Z) = C*(sin Z + cos Z)*(Z^3+Z+C)

42--F(Z) = Cexp(Z) * exp(cosCZ)

43--F(Z) = (Z^3+Z+C)*C*(sinZ + cosZ)

44--F(Z) = ((1+C)Z-CZ^2)*((Z+sinZ)^2+C)

45--F(Z) = Z^2 + Z^1.5 + C

46--F(Z) = Z^2 + ZexpZ + C

47--F(Z) = (Z+sinZ)^2+Cexp(-Z)+Z^2+C

48--F(Z) = ((Z^3)/(1+CZ^2))+expZ-C

49--F(Z) = (Z^2*sin(ReZ) + CZ(ImZ) + (Z^2*cos(ReZ)+CZsin(ImZ)+C

50--F(Z) = (Z+sinZ)^2+Cexp(Z)+C

51-- F(Z) = Z^2 + 1/Z + C

52-- F(Z) = (Z^3 + C) / Z

53-- F(Z) = (Z^3 + C) / Z^2

54-- F(Z) = ((Z+1)^2 + C) / Z

55-- F(Z) = (Z + C)^2 + (Z + C)*

56-- F(Z) = (Z + C)^3 - (Z + C)^2

57-- F(Z) = (Z^3 - Z^2)^2 + C

58-- F(Z) = (Z^2 - Z)^2 + C

59-- F(Z) = (Z + ln Z)^2 + C

60-- F(Z) = (Z - sqrt(Z))^2 + C

61-- F(Z) = (Z + sqrt(Z))^2 + C

62-- F(Z) = Z^2exp(Z) - Zexp(Z) + C

63-- F(Z) = (exp(CZ) + C)^2

64-- F(Z) = Z * exp(Re Z/Im Z) + C

65-- F(Z) = exp(X^2*Y^2) + Im Z + C

66-- F(Z) = exp(Re Z)*(X-a) + exp(Im Z)*(Y-b)i

67-- F(Z) = X^2*exp(Y+b) + iaexp(Y+b)

68-- F(Z) = (a-X^2+Y^2)exp(b+X^2-Y^2) + i(b+X^2-Y^2)exp(a-X^2+Y^2)

69-- F(Z) = [(2X-Y^2+a)/(2X^2+Y-b)] + i[(2X^2+Y-a)/(2X-Y^2+b)]

70-- F(Z) = [(X^2+Y^2+a)/cos(X^2+Y^2)] + i[(X^2+Y^2+b)/sin(X^2+Y^2)]

71-- F(Z) = Z^5 + C

72-- F(Z) = Z^6 + C

73-- F(Z) = Z^7 + C

74-- F(Z) = (3Z^4 + C) / 4Z^3

75-- F(Z) = (2Z^3 + C) / 3Z^2

76-- F(Z) = Z^5 + CZ^3 + C

77-- F(Z) = Z^6 + CZ^4 + CZ^2 + C

78-- F(Z) = Z^8 + C

79-- F(Z) = Z^9 + C

80-- F(Z) = Z^8 + CZ^4 + CZ^2 + C

81-- F(Z) = Z^9 - CZ^6 + CZ^3 + C

82-- F(Z) = (Z^4 + C) / (Z - C)

83-- F(Z) = (Z^3 + Z + C) / (Z^2 - Z - C)

84-- F(Z) = (Z^3 + Z + C) / (Z - C)

85-- F(Z) = (Z^3 + Z + C) / Z

86-- X = X^2+XY+A ; Y = Y^2-XY+B

87-- X = X^3-(X^2)Y+XY^2-XY+A; Y = Y^3-XY^2+(X^2)Y+XY+B

88-- X = (X^2)sin Y + A ; Y = (Y^2)cos X + B

89-- X = X^4-3X^3+3X^2(Y^2)+A ; Y = Y^4+3XY^3-3X^2(Y^2)

90-- X = X^2(1+exp(-Y))+A ; Y = Y^2(1+exp(-X)+B

91-- F(Z) = C(Z^2 + 1)^2 / Z(Z^2 -1)

92-- F(Z) = CZ^2

93-- F(Z) = CZ^3

94-- F(Z) = CZ^4

95-- F(Z) = C*cos Z

96-- F(Z) = C*sin Z

97-- F(Z) = CZ*ln Z

98-- F(Z) = C*tan Z

99-- F(Z) = C*exp(CZ) / (exp(C) - 1)

100-- F(Z) = C*exp(Z)*sqrt(Z) /n

101 -- F(Z) = (Z^2(1+Z^2))/(Z+C)

102 -- F(Z) = Z(1+Z^2)/(Z+C)

103 -- F(Z) = (Z^5+C)/(Z^3+Z^2+Z+1)

104 -- F(Z) = (Z^3+C)/3Z^2

105 -- F(Z) = (Z^3+Z^2+Z+C)/(Z-C)

106 -- F(Z) = exp(Z^2+C)

107 -- F(Z) = Z^2*exp(Z^2)+C

108 -- F(Z) = exp(Z^2)/(Z+C)

109 -- F(Z) = (Z+exp(Z))^2+C

110 -- F(Z) = (Z^2+C)^2-exp(Z)+C

111 -- F(Z) = (1+iC)sin(Z)

112 -- F(Z) = (1+iC)cos(Z)

113 -- F(Z) = Z*tan(ln Z)+C

114 -- F(Z) = sqrt(Z^4+1)+C

115 -- F(Z) = sqrt(Z^4+C)

116 -- F(Z) = C^Z

117 -- F(Z) = C*arctan(Z)

118 -- F(Z) = (ZlnZ)/exp(C)

119 -- F(Z) = exp(Z)/lnZ+C

120 -- F(Z) = sqrt(Z^3+C)

121 -- F(Z) = sqrt(Z^3+1)+C

122 -- F(Z) = cubrt(Z^6+1)+C

123 -- F(Z) = (Z+exp(Z)+ln Z)^2+C

124 -- F(Z) = (Z^2+C+1)^2 / (2Z+C+2)^2

125 -- F(Z) = Z ^ 10 + C

126 -- F(Z) = Z ^ 11 + C

127 -- F(Z) = Z ^ 12 + C

128 -- F(Z) = Z^12 - Z^11 - Z^10 + C

129 -- F(Z) = Z ^ 13 + C

130 -- F(Z) = Z ^ 14 + C

131 -- F(Z) = Z ^ 15 + C

132 -- F(Z) = Z ^ 16 + C

133 -- F(Z) = Z ^ 17 + C

134 -- F(Z) = Z ^ 18 + C

135 -- F(Z) = Z ^ 19 + C

136 -- F(Z) = Z ^ 20 + C

137 -- F(Z) = Z ^ 21 + C

138 -- F(Z) = Z ^ 22 + C

139 -- F(Z) = Z ^ 23 + C

140 -- F(Z) = Z ^ 24 + C

141 -- F(Z) = Z ^ 25 + C

142 -- F(Z) = Z ^ 26 + C

143 -- F(Z) = Z ^ 27 + C

144 -- F(Z) = Z ^ 28 + C

145 -- F(Z) = Z ^ 29 + C

146 -- F(Z) = Z ^ 30 + C

147 -- X=X^2+Y+A+X^2/Y ;Y=Y^2+X+B+Y^2/X

148 -- X=X^3+Y^2-X+A ;Y=Y^3-X^2+Y+B

149 -- X=X^2+2XY-Y+A ;Y=Y^2-2XY+X+B

150 -- X=X^3+AX^2+BY ;Y=Y^3+BY^2+AX

151 -- X=2X^2-3ABY+A ;Y=3Y^2+2ABX-B

152 -- X=X^4lnX+Y^2sinY+A; Y=Y^4lnY+X^2cosX+B

153 -- X=sqr(ln(X^2))+YsinX+A; Y=sqr(ln(Y^2))-XcosY+B

154 -- X=.5(X^2-Y^2)+.5(X+Y)+A; Y=.5(Y^2-X^2)-.5(X+Y)+B

155 -- X=sqr(X^3)+sqr(Y^3)+A; Y=sqr(Y^3)-sqr(X^3)+B

156 -- X=Y/sqrX+X/sqrY+A; Y=XsqrY+YsqrX+B

157 -- F(Z) = Z^30 - 30Z^29 - 870Z^28 + C

158 -- F(Z) = Z^27 - 27Z^26 - 702Z^25 + C

159 -- F(Z) = Z^24 - 24Z^23 - 552Z^22 + C

160 -- F(Z) = Z^21 - 21Z^20 - 420Z^19 + C

161 -- F(Z) = Z^18 - 18Z^17 - 306Z^16 + C

162 -- F(Z) = Z^15 - 15Z^14 - 210Z^13 + C

163 -- F(Z) = Z^30 - 30Z^29 - 870Z^28 + Z^27 - 27Z^26 - 702Z^25 + C

164 -- F(Z) = Z^27 - 27Z^26 - 702Z^25 + Z^24 - 24Z^23 - 552Z^22 + C

165 -- F(Z) = Z^24 - 24Z^23 - 552Z^22 + Z^21 - 21Z^20 - 420Z^19 + C

166 -- F(Z) = Z^21 - 21Z^20 - 420Z^19 + Z^18 - 18Z^17 - 306Z^16 + C

167 -- F(Z) = Z^18 - 18Z^17 - 306Z^16 + Z^15 - 15Z^14 - 210Z^13 + C

168 -- F(Z) = Z^30 - 30Z^29 - 870Z^28 + Z^27 - 27Z^26 - 702Z^25 + Z^24 - 24Z^23 -
552Z^22 + C

169 -- F(Z) = Z^27 - 27Z^26 - 702Z^25 + Z^24 - 24Z^23 - 552Z^22 + Z^21 - 21Z^20 -
420Z^19 + C

170 -- F(Z) = Z^24 - 24Z^23 - 552Z^22 + Z^21 - 21Z^20 - 420Z^19 + Z^18 - 18Z^17 -
306Z^16 + C

171 -- F(Z) = Z^21 - 21Z^20 - 420Z^19 + Z^18 - 18Z^17 - 306Z^16 + Z^15 - 15Z^14 -
210Z^13 + C

172 -- F(Z) = Z^30 - Z^29 + Z^28 - Z^27 + Z^26 - Z^25 + C

173 -- F(Z) = Z^24 - Z^23 + Z^22 - Z^21 + Z^20 - Z^19 + C

174 -- F(Z) = Z^18 - Z^17 + Z^16 - Z^15 + Z^14 - Z^13 + C

175 -- F(Z) = Z^15sinX - Z^14cosY - Z^13tanX + C

176 -- F(Z) = Z^12cosX - Z^11sinY - Z^10tanY + C

177 -- F(Z) = Z^15sinA - Z^14cosB - Z^13tanX - Z^12tanY + C

178 -- F(Z) = Z^12cosA - Z^11sinB - Z^10tanY - Z^9tanX + C

179 -- F(Z) = Z^30sinX - 30Z^29cosY + C

180 -- F(Z) = Z^28cosX - 28Z^27sinY + C

181 -- F(Z) = (Z^3+3Z(C-1)+(C-1)(C-2))^2

182 -- F(Z) = (3Z^2+3Z(C-2)+C^2-3C+3)^2

183 -- F(Z) = (Z^3+3Z(C-1)+(C-1)(C-2))^2 / (3Z^2+3Z(C-2)+C^2-3C+3)^2

184 -- F(Z) = Z ^ pi + C

185 -- F(Z) = pi ^ Z + C

186 -- F(Z) = Z ^ 4 + C

187 -- F(Z) = Z ^ pi + pi ^ C

188 -- F(Z) = C * Z ^ pi

189 -- F(Z) = Z ^ pi - Z ^ 3 + C

190 -- F(Z) = Z ^ pi - Z ^ 2 + C

191 -- F(Z) = Z ^ 2.5 + C

192 -- F(Z) = (5Z^6 + C)/6Z^5

193 -- F(Z) = Z ^ e + C

194 -- F(Z) = Z ^ (C * e)

195 -- F(Z) = (Z ^ e) ^ C

196 -- F(Z) = C * Z ^ e

197 -- F(Z) = Z ^ (pi * e)

198 -- F(Z) = Z * (C ^ e)

199 -- F(Z) = cbrt(Z ^ 7 + 1) + C

200 -- F(Z) = Z ^ 4.669 + C

201 -- F(Z) = (Z ^ 8 + 1) ^ 1/4 + C

202 -- F(Z) = (Z ^ 9 + 1) ^ 1/4 + C

203 -- F(Z) = ((Z ^ 2 * (ReZ - (ImZ)^2))/(1 - Z)) + C

204 -- F(Z) = (Z ^ 10 + C) ^ 1/4

205 -- F(Z) = (Z ^ 10 + 1) ^ 1/4 + C

206 -- F(Z) = (Z ^ 11 + C) ^ 1/4

207 -- F(Z) = (Z ^ 11 + 1) ^ 1/4 + C

208 -- F(Z) = (Z ^ 12 + C) ^ 1/4

209 -- F(Z) = (Z ^ 12 + 1) ^ 1/4 + C

210 -- F(Z) = YZ^2sinX - XZcosY + C

211 -- F(Z) = XZ^3cosY + YZ^2sinX + C

212 -- F(Z) = Z^4 - Z^2cosX + YsinY + C

213 -- F(Z) = XYZ^2 + C

214 -- F(Z) = Z^2 + X^2*Y^2 + C

215 -- F(Z) = Z^3 + X^2sinY + Y^2cosX + C

216 -- F(Z) = (Z ^ 13 + C) ^ 1/6

217 -- F(Z) = (Z ^ 5 + C) ^ 1/3

218 -- F(Z) = (Z ^ 4 + C) ^ 1/sin X

219 -- F(Z) = Z ^ 2 + iZ ^ 2 + C

220 -- F(Z) = Z ^ 3 + iZ ^ 3 + C

221 -- F(Z) = Z ^ 4 + iZ ^ 2 + C

222 -- F(Z) = (Z ^ 4 / Z + 1) + C

223 -- F(Z) = (Z ^ 6 / Z + 1) + C

224 -- F(Z) = (Z ^ 4 / Z + i) + C

225 -- F(Z) = (Z ^ 6 / Z + i) + C

226 -- F(Z) = (Z ^ 2 / (lnZ)^2) + C

227 -- F(Z) = (Z ^ 2 / (ln(Z^2)) + C

228 -- F(Z) = (Z ^ 3 / (lnZ)^3) + C

229 -- F(Z) = (Z ^ 3 / (ln(Z^3)) + C

230 -- F(Z) = (Z ^ 4 / (lnZ)^4) + C

231 -- F(Z) = (Z ^ 4 / (ln(Z^4)) + C

232 -- F(Z) = Z ^ 2 + Z / ln Z + C

233 -- F(Z) = Z ^ 2 + ln Z / Z + C

234 -- F(Z) = Z ^ 6 + Z ^ 4 + Z ^ 2 + C

235 -- F(Z) = Z ^ 6 - Z ^ 4 - Z ^ 2 + C

236 -- F(Z) = Z ^ (1/Z) + C

237 -- F(Z) = Z ^ 2 + sin Z / Z + C

238 -- F(Z) = Z ^ 2 + Z / sin Z + C

239 -- F(Z) = Z ^ iZ + C

240 -- F(Z) = Z ^ 2 * exp(X) + C

241 -- F(Z) = Z ^ 2 * exp(X ^ 2) + C

242 -- F(Z) = Z ^ 3 * exp(X) + Z ^ 2 * exp(Y) + C

243 -- F(Z) = exp(Z ^ Z) + C

244 -- F(Z) = (Z ^ 3) / (Z + 1) + C

245 -- F(Z) = Z ^ 2 / C

246 -- F(Z) = (Z ^ 4 + 1) / (Z + C)

247 -- F(Z) = (Z ^ 4 + C) / (Z ^ 2 + 1)

248 -- F(Z) = (Z ^ 4 + C) / (1 - Z ^ 2)

249 -- F(Z) = Z ^ 2 * exp(Z) / (Z + C)

250 -- F(Z) = Z ^ 2 - exp(Z) + sin(Z) + C

251 -- F(Z) = (Z ^ 4) / (Z ^ 2 + C)

252 -- F(Z) = Z ^ 2 + sqrt(Z ^ 2 + C)

253 -- F(X) = X^2 - Y^2 + XsinY + A; F(Y) = Y^2 - B

254 -- F(X) = X^2 + atan(Y/X) + A; F(Y) = Y^2 - A

255 -- F(X) = 1 - X - Y^2 + A; F(Y) = 1 - Y + X^2 + B

256 -- F(X) = exp(sqrt(X)) - exp(sqrt(Y)) + A; F(Y) = exp(XlnY) + B

257 -- F(Z) = C ^ 2 * ln(Z ^ 2)

258 -- F(Z) = Z ^ 2 ln(C)

259 -- F(Z) = Z ^ 2 ln(C) + C

260 -- F(Z) = Z ^ 2 ln(Z + C)

261 -- F(Z) = Z ^ -2 + C

262 -- F(Z) = ((X^2 + Y^2 + A) / (X^2 - Y^2)) + i[((X^2 - Y^2 - B) / (X^2 + Y^2))]

263 -- F(Z) = (X^3 - iY + C) / (X + Y + 1)

264 -- F(Z) = [(X^2 + A^2) / Y] + i[(Y^2 + B^2) / X]

265 -- F(Z) = [(X^3 + X^2 + X + A) / (Y^3 - Y^2 - Y - 1)] + i[(Y^3 + Y^2 + Y + B) /
(X^3 - X^2 - X - 1)]

266 -- F(Z) = [(X^4 - Y^2) / (X + Y + A)] + i[(X^2 + Y^4) / (X - Y - B)]

267 -- F(Z) = C ^ 3 / Z ^ 2

268 -- F(Z) = [Z^(1/2) / Z^(1/3)] + C

269 -- F(Z) = (Z ^ 2 + C) / (1 - C)

270 -- F(Z) = (exp(Z ^ 4)/ Z ^ 4) + C

271 -- F(Z) = (Z ^ 6 + 1) ^ (1/5) + C

272 -- F(Z) = Z ^ 2 + CZ + C * sin Y - Z * cos X + C

273 -- F(Z) = Z ^ 6 - Z ^ 5 - Z ^ 4 - Z ^ 3 - Z ^ 2 - Z + C

274 -- F(Z) = Z ^ 2 * (sin C / C)

275 -- F(Z) = exp(- Z ^ 2 / 2) + C

276 -- F(Z) = (Z ^ 3 + 3 * Z - 1) / (2 - Z)

277 -- F(Z) = Z ^ 3 * sin C + Z ^ 2 * cos C + XY + C

278 -- F(Z) = (Z ^ 2 + 1) ^ 2 / (Z + C) ^ 2

279 -- F(Z) = (Z ^ 2 + C + 1) ^ 2 / (Z - C - 1) ^ 2

280 -- F(Z) = Z ^ 4 * sin Y + Z ^ 2 * cos X + XY + C

281 -- F(Z) = Z * cos (XY) + C

282 -- F(Z) = Z ^ 2 * cos (X ^ 2 + Y ^ 2) + C

283 -- F(Z) = Z ^ (2 + ln C)

284 -- F(Z) = Z ^ (9/7) + C

285 -- F(Z) = Z ^ 5 * (1 - Z - (Z + C) ^ 2) + C

286 -- F(Z) = Z ^ 6 + Z ^ 5 + C

287 -- F(Z) = Z ^ 6 + Z ^ 4 + C

288 -- F(Z) = Z ^ 6 + Z ^ 3 + C

289 -- F(Z) = Z ^ 6 + Z ^ 2 + C

290 -- F(Z) = Z ^ 6 + Z + C

291 -- F(Z) = Z ^ 2 + cos Z + C

292 -- F(Z) = Z ^ 2 + cos 2Z + C

293 -- F(Z) = Z ^ 2 + cos 3Z + C

294 -- F(Z) = Z ^ 2 + cos 4Z + C

295 -- F(Z) = Z ^ 2 + cos 5Z + C

296 -- F(Z) = (Z ^ 7 + C) / Z ^ 5

297 -- F(Z) = (Z ^ 7 + C) / Z ^ 4

298 -- F(Z) = (Z ^ 7 + C) / Z ^ 3

299 -- F(Z) = (Z ^ 7 + C) / Z ^ 2

300 -- F(Z) = (Z ^ 7 + C) / Z

301 -- F(Z) = Z ^ 3 - Z ^ 2 - Z + C

302 -- F(Z) = Z ^ 4 - Z ^ 3 - Z ^ 2 + C

303 -- F(Z) = Z ^ 5 - Z ^ 4 - Z ^ 3 + C

304 -- F(Z) = Z ^ 6 - Z ^ 5 - Z ^ 4 + C

305 -- F(Z) = Z ^ 7 - Z ^ 6 - Z ^ 5 + C

306 -- F(Z) = Z ^ 2 * (cos(Z)) ^ 2 + C

307 -- F(Z) = Z ^ 2 * (cos(XY)) ^ 2 + C

308 -- F(Z) = Z ^ 4 * (sin(Z)) ^ 2 + C

309 -- F(Z) = Z ^ 3 * (sin(XY)) ^ 2 + C

310 -- F(Z) = Z ^ 3 * (cos(Z)*sin(Z)) + C

311 -- F(Z) = (Z ^ 2 / sin(Z)) + C

312 -- F(Z) = (Z ^ 4 / cos(Z)) + C

313 -- F(Z) = (Z ^ 6 + C) / (sin(Z) * cos(Z))

314 -- F(Z) = (Z ^ 3 + Z ^ 2 + Z + C) / (Z + cos(Z)

315 -- F(Z) = (Z ^ 2 * ln Z + Z + C) / (sin(Z)) ^ 2

316 -- F(Z) = Z ^ 4 + (cos X) ^ 2 + (sin Y) ^ 2 + C

317 -- F(Z) = Z ^ 3 + cos X * sin Y + C

318 -- F(Z) = Z ^ 4 + Z + cos C

319 -- F(Z) = Z ^ 2 + Z + tan C

320 -- F(Z) = Z ^ 3 + Z ^ 2 + exp(1 + sin X) + C

321 -- F(Z) = sqrt(Z ^ 4 + cos(theta) + C); theta = arctan (Im Z / Re Z)

322 -- F(Z) = sqrt(Z ^ 5 + Z ^ 3 + Z + C)

323 -- F(Z) = sqrt(Z ^ 4 + Z ^ 3 + Z ^ 2 + Z + C)

324 -- F(Z) = sqrt(Z ^ 6 - Z ^ 3 + C)

325 -- F(Z) = sqrt(ln (Z ^ 2) + Z ^ 2 * ln Z + C)

326 -- F(Z) = cos((Z ^ 2 + C) / XY)

327 -- F(Z) = cos((Z ^ 3 + C) / XY)

328 -- F(Z) = cos((Z ^ 4 + C) / XY)

329 -- F(Z) = ((Z ^ 4 + C) / XY) + cos((Z ^ 3 + C) / XY)

330 -- F(Z) = cos((Z ^ 4 + C) / XY) + cos((Z ^ 3 + C) / XY) + cos((Z ^ 2 + C) / XY)

331 -- F(Z) = Z ^ 3/2 + Z ^ 4/3 + C

332 -- F(Z) = Z ^ 4/3 + Z ^ 5/4 + C

333 -- F(Z) = Z ^ 5/4 + Z ^ 6/5 + C

334 -- F(Z) = Z ^ 5/2 + Z ^ 7/3 + C

335 -- F(Z) = Z ^ (pi/e) ^ 2 + C

336 -- F(Z) = Y * sin X * cos Y * exp(-X) + C

337 -- F(Z) = Z ^ 2 * cos X * cos Y * exp(-Y) + C

338 -- F(Z) = XYZ * sin X * sin Y * exp(Z) + C

339 -- F(Z) = Z ^ 3 + X ^ 2 * Y ^ 2 * cos X * sin Y + C

340 -- F(Z) = Z ^ 2 + X ^ 2 * sin Y + Y ^ 2 * cos X + C

341 -- F(Z) = 1 / Z + 1 / Z ^ 2 + C

342 -- F(Z) = Z ^ 2 / Z' + Z ^ 3 / Z' ^ 2 + C

343 -- F(Z) = Z ^ 3 / C' + Z ^ 2 + C

344 -- F(Z) = Z ^ 2 + Z' ^ 2 + C

345 -- F(Z) = Z ^ 3 + Z ^ 2 * Z' + Z * Z' ^ 2 + Z' ^ 3 + C

346 -- F(Z) = Z ^ 4 - Z ^ 3 * Z' + Z ^ 2 - Z' + C

347 -- F(Z) = Z ^ 5 - C * Z ^ 3 - C' * Z ^ 2 + Z' + C

348 -- F(Z) = Z ^ 4 * Z' ^ 2 - Z ^ 3 * Z' + C

349 -- F(Z) = Z ^ 6 + Z' ^ 5 + Z ^ 4 + Z' ^ 3 + Z ^ 2 + Z' + C

350 -- F(Z) = Z ^ 4 + Z ^ 2 / Z' + Z' ^ 3 / Z ^ 2 + C

351 -- F(Z) = arcsin(ln(Z)) + C

352 -- F(Z) = arctan(ln(Z)) + C

353 -- F(Z) = (arcsin(ln(Z))) ^ 2 + C

354 -- F(Z) = e ^ (1 + cos(ln(Z))) + C

355 -- F(Z) = e ^ (2 - e ^ cos(Z)) + C

356 -- F(Z) = XY * Z^2 - X^2 * YZ + X * Y ^ 2 * Z ^ 3 + C

357 -- F(Z) = X ^ 3 * Y ^ 4 + X ^ 2 * Z ^ 5 + C

358 -- F(Z) = XY^2Z^3 - X^3Y^2Z + X^2Y^2Z^2 + C

359 -- F(Z) = Z ^ 4 - X ^ 2 * cos(Y) + Y * sin(X) + C

360 -- F(Z) = Z ^ 3 - Y ^ 2 * cos(XY) - X ^ 2 * sin(X) - Y * cos(Y) + C

361 -- F(Z) = (Z ^ 3 + C) / (Z ^ 3 - C)

362 -- F(Z) = (Z ^ 3 + C ^ 2 + 1) / (Z ^ 3 - C ^ 2 - 1)

363 -- F(Z) = (Z ^ 3 + Z + C) / (Z ^ 3 - Z - 1)

364 -- F(Z) = (Z ^ 2 - Z ^ 3 + 1) / (Z ^ 4 + C)

365 -- F(Z) = (Z ^ 4 + C) / (4Z ^ 3 + 1)

366 -- F(Z) = (Z ^ C) / (Z + 1)

367 -- F(Z) = (Z ^ (1 + C)) / (1 + C)

368 -- F(Z) = (2 ^ Z) / C

369 -- F(Z) = 2 ^ Z + C

370 -- F(Z) = 2 ^ Z + (2 ^ Z) / C + C

371 -- F(Z) = XYZ ^ 2 - X ^ 2YZ + C

372 -- F(Z) = X ^ 4 * Y ^ 3 * Z ^ 2 + C

373 -- F(Z) = X^3*Y^3*Z^3 - X^2*Y^2*Z^2 + XYZ + C

374 -- F(Z) = XY^2Z + X^2YZ^4 + C

375 -- F(Z) = Z^2*sqrt(XY) + XY^2Z^4*sqrt(XY) + C

376 -- F(Z) = Z ^ (2XY) + C

377 -- F(Z) = X ^ (2YZ) + C

378 -- F(Z) = Y ^ (Z^2) + X + C

379 -- F(Z) = X ^ (2YZ) + Z ^ (2XY) + C

380 -- F(Z) = (XY) ^ (Z - C)

381 -- F(Z) = Z ^ 2C + C

382 -- F(Z) = Z ^ 2 + C ^ 2Z + C

383 -- F(Z) = X^Y + Z^X + Y^Z + C

384 -- F(Z) = Z ^ 2 + A ^ X + B ^ Y + C

385 -- F(Z) = Z ^ 3 + X ^ (AB) + Y ^ C

386 -- F(Z) = Z ^ 9 - Z ^ 8 - Z ^ 7 + C

387 -- F(Z) = Z^9 - 9Z^8 - 8Z^7 + C

388 -- F(Z) = Z^9 - 9Z^8 - 8Z^7 - 7Z^6 - 6Z^5 - 5Z^4 + C

389 -- F(Z) = Z^9 - 9Z^8 - 8Z^7 - 7Z^6 - 6Z^5 - 5Z^4 - 4Z^3 - 3Z^2 - 2Z +C

390 -- F(Z) = Z^9 + C^9

391 -- F(Z) = Z^3 + Z^2 + CsinX + C

392 -- F(Z) = Z^4 + X^2 - Y^2 - C^2*cosZ + C + A

393 -- F(Z) = Z^5 + Im(Z^4 + Z^3 + Z^2) + CZRe(Z^2 + C) + C

394 -- F(Z) = Z^3 + Z^2*cosY + ZsinX + C

395 -- F(Z) = Z^4 + (Z^2 / sinY) + (CZ^3 / cosX) + C

396 -- F(Z) = (Z + ln Z)^4 + C

397 -- F(Z) = Z + (ln Z)^4 + C

398 -- F(Z) = Z^2 + (ln Z)^3 + C

399 -- F(Z) = Z^3 + (ln Z)^2 + C

400 -- F(Z) = (ln Z)^2 + C^2 + C

401 -- F(Z) = Z^2 + C + A

402 -- F(Z) = Z^2 + C + iB

403 -- F(Z) = Z^2 + C + X

404 -- F(Z) = Z^2 + C + iY

405 -- F(Z) = Z^2 + C + iXY

406 -- F(Z) = X^3 + X^2Y - XY^2 + Y^3 + C

407 -- F(Z) = X^5 + iX^4 -iX^3Y + iX^2Y^2 - iXY^3 + iY^4 + C

408 -- F(Z) = Y^3 - Y^2 - Y - 1 - A + iX^3 + iX^2 + iX + i + iB

409 -- F(Z) = Y^4 + Y^2 + A - iX^4 - iX^2 - iB

410 -- F(Z) = X^2 + X + 1 + A + iY^2 - iY - i - iB

411 -- F(Z) = arcsin(Z) + C (3rd appr)

412 -- F(Z) = 1 - Z/X - Z^2/Y + C

413 -- F(Z) = arctan(Z) + C (5th appr)

414 -- F(Z) = X^3/Y^2 + Y^4/X^3 + A + i(Y^2/X) - i(X^3/Y) + iB

415 -- F(Z) = Z^4/(X+Y) + Z^3/(X-Y) + C

416 -- F(Z) = Z^(2-X) + C

417 -- F(Z) = Z^(2-X-Y) + C

418 -- F(Z) = Z^(3+C)

419 -- F(Z) = Z^(2X^2 - 3Y^2) + C

420 -- F(Z) = (X+Y)^2Z + C

421 -- F(Z) = Z^2 + sin(Z)*cos(Z) + C

422 -- F(Z) = Z^2 + sec(Z)*tan(Z) + C

423 -- F(Z) = Z^2 + sin(Z)*tan(Z) + C

424 -- F(Z) = Z^2 + cot(Z)*arcsin(Z) + C

425 -- F(Z) = Z^2 + tan(Z)*arccos(Z) + C

426 -- F(Z) = Z^(2-Z) + C

427 -- F(Z) = Z^(3-Z) + C

428 -- F(Z) = Z^(4-Z) + C

429 -- F(Z) = Z^(5-Z) + C

430 -- F(Z) = Z^(6-Z) + C

431 -- F(Z) = Z^(2-C) + C

432 -- F(Z) = Z^(3-C) + C

433 -- F(Z) = Z^(4-C) + C

434 -- F(Z) = Z^(5-C) + C

435 -- F(Z) = Z^(6-C) + C

436 -- F(Z) = Z^Z / Z^C

437 -- F(Z) = C^Z / Z^Z

438 -- F(Z) = (1-C)^2Z

439 -- F(Z) = (Z+C)^Z

440 -- F(Z) = (Z^2 + C^2)^2Z

441 -- F(Z) = Z^CZ

442 -- F(Z) = Z^(C^2) + C

443 -- F(Z) = C^(2^Z) + C

444 -- F(Z) = Z^(tan(Z) + C

445 -- F(Z) = Z^(sin(Z)cos(Z)) + C

446 -- F(Z) = 2CZ / (Z + C)

447 -- F(Z) = 2CZ / sqrt(Z + C)

448 -- F(Z) = 2 * Z^2 * C^2 / (Z + C)

449 -- F(Z) = 2CZ^3 / (Z + C)

450 -- F(Z) = sqrt(2CZ) / (Z + C)

451 -- F(Z) = Z ^ (Z/C)

452 -- F(Z) = Z^2 + Z ^ (Z/C)

453 -- F(Z) = Z ^ (Z/C) + Z + C

454 -- F(Z) = Z ^ (Z/C) Z ^ 2 + C

455 -- F(Z) = Z ^ (Z^2 / C)

456 -- F(Z) = Z ^ (C/Z)

457 -- F(Z) = Z ^ (C/Z) + Z

458 -- F(Z) = Z ^ (C/Z) + Z^2

459 -- F(Z) = Z ^ (C/Z) + C

460 -- F(Z) = Z ^ (C^2 / Z)

461 -- F(Z) = Z ^ ln(Z ^ Z/C)

462 -- F(Z) = Z ^ ln(Z ^ C/Z)

463 -- F(Z) = Z ^ Z/C + Z ^ C/Z

464 -- F(Z) = sqrt(X^2 + Y^2) + iarctan(Y/X) + C

465 -- F(Z) = Z^2 + sqrt(X^2 + Y^2) + iarctan(Y/X) + C

466 -- F(Z) = Z^3 + sqrt(X^2 + Y^2) + iarctan(Y/X) + C

467 -- F(Z) = Z^4 + sqrt(X^2 + Y^2) + iarctan(Y/X) + C

468 -- F(Z) = Z^2 + sqrt(A^2 + B^2) + iarctan(B/A)

469 -- F(Z) = Z^3 + sqrt(X^3 + Y^3) + C

470 -- F(Z) = Z^4 + sqrt(X^4 + Y^4) + C

471 -- F(Z) = Z^5 + sqrt(X^5 + Y^5) + C

472 -- F(Z) = Z^6 + sqrt(X^6 + Y^6) + C

473 -- F(Z) = Z^7 + sqrt(X^7 + Y^7) + C

474 -- F(Z) = Z^8 + sqrt(X^8 + Y^8) + C

475 -- F(Z) = Z^9 + sqrt(X^9 + Y^9) + C

476 -- F(Z) = sqrt(X^2 + Y^2) + isqrt(X^3 + Y^3)

477 -- F(Z) = sqrt(X^3 + Y^3) + isqrt(X^4 + Y^4)

478 -- F(Z) = sqrt(X^4 + Y^4) + isqrt(X^5 + Y^5)

479 -- F(Z) = sqrt(X^5 + Y^5) + isqrt(X^6 + Y^6)

480 -- F(Z) = sqrt(X^6 + Y^6) + isqrt(X^7 + Y^7)

481 -- F(Z) = Z^2 + exp(cot(Z))*cot(Z)

482 -- F(Z) = Z^2 + exp(tan(Z))*tan(Z)

483 -- F(Z) = Z^2 + exp(cos(Z))*cos(Z)

484 -- F(Z) = Z^2 + exp(sin(Z))*sin(Z)

485 -- F(Z) = Z^2 + (exp(cot(Z))/ Z) + C

486 -- F(Z) = Z * det|X A Y B| + i * det|A Y B X| + C

487 -- F(Z) = Z^2 + det|X A Y B| + C

488 -- F(Z) = Z^2 * C^2 * det|X A Y B| + C

489 -- F(Z) = Z^3 * C^3 * det|X A Y B| - C

490 -- F(Z) = 2XY - i(X^2 - Y^3) + C

491 -- F(Z) = 3*X^3*Y^2 - iZ^2 + C

492 -- F(Z) = ZC^3 - Z^2*C^2 - CZ^3 + C\n");

493 -- F(Z) = X^2*Y*Z^2 - Y^2*Z*sin(X) + X^2*cos(Y) + C

494 -- F(Z) = Y^3*Z^3 - ZX^2 - C^2 * sin(Y) + C

495 -- F(Z) = X^2*Y^2*Z^2*C^2 + CXYZ + iZ^3

496 -- F(Z) = X^3*Y^3*Z^3 + iCXZ^2

497 -- F(Z) = X^2*Y^8*Z^5 + iXYZC^4

498 -- F(Z) = X^2*Y^3*Z^4 + XY^2*Z^3 + Z^2 + C

499 -- F(Z) = XYZ^2*cos(X) + X^2 - Y^2 + BCZ + C

500 -- F(Z) = Z^2 + ABXY + C

The next fifty-two equations are exhibited
in the 2005 "M" line of fractal imagery.

501 -- F(Z) = Z^C + SIN C

502 -- F(Z) = (SQRT Z + C) / C

503 -- F(Z) = (SIN(Z+1))^Z * COS(1/Z) + C

504 -- F(Z) = SIN(Z * COS Z + C) + C

505 -- F(Z) = COS(Z^2 / C) + SIN(C / Z^2) + C

506 -- F(Z) = Z^C + C^Z + C^(Z^2) + Z^(C^2)

507 -- F(Z) = ((Z + SIN(Z) + C)^2 + C) / Z

508 -- F(Z) = SIN(COS(Z^2 + C) + Z + C

509 -- F(Z) = SIN(Z^2) * LOG(C^2) * (Z * C^(SQRT(Z)) + C

510 -- F(Z) = Z^2 + Z * C^(SQRT(Z)) + C

511 -- F(Z) = SIN(Z^2 / C) + COS(Z / C) + Z^2 + C

512 -- F(Z) = ((Z^4 + C) / (Z^2 - C)) + Z^2 + C

513 -- F(Z) = ((Z^2 + C)^2 + Z - C^3) / 2(Z^2 + C)

514 -- F(Z) = e^(Z^2) + e^2Z - Z^2 - 1 + C

515 -- F(Z) = (2e^2Z / Z^3) + C

516 -- F(Z) = 3Z^2 * 3^(Z^3) - 3^Z + C

517 -- F(Z) = (1 + LOG(Z))^3 + C

518 -- F(Z) = (Z + 1/Z)^2.5 + C

519 -- F(Z) = (Z^(Z - 1) + 1)^2 + C

520 -- F(Z) = (1 / LOG(Z + C))

521 -- F(Z) = C * (Z + 1/Z) + Z^(-.5) + C

522 -- F(Z) = Z^2 + Z^1.75 + Z^1.5 + Z^1.25 + Z + C

523 -- F(Z) = ((Z^4 + Z^2 + C)^2 / (Z^5 + Z^3 + Z + C))

524 -- F(Z) = (1 / SINH(1 / Z^2)) + C

525 -- F(Z) = (Z ^ C + Z) / C

526 -- F(Z) = (Z + C^Z) / C

527 -- F(Z) = (Z^C + C) / Z

528 -- F(Z) = (C^Z + C) / Z

529 -- F(Z) = Z^1.75 + C

530 -- F(Z) = (Z^2.5 / LOG(Z)) + C

531 -- F(Z) = Z^2 * LOG(Z) - C*Z + Z + C

532 -- F(Z) = SQRT(Z^6 + Z + C) + C

533 -- F(Z) = (C * Z^2)^Y + C

534 -- F(Z) = SQRT(Z^4 + Z^3) + Z + C

535 -- F(Z) = (((Z^2 + X - 1)^2) / (2Z + X + 1)^2) + C

536 -- F(Z) = Z^2 + X + Y - X^2 * Y^2 + C

537 -- F(Z) = Z^(Z^2 + C) - Z + C

538 -- F(Z) = (Z + TAN(Z) + TAN(1/Z))^2 + C

539 -- F(Z) = Z^(C - 1) * (1 - Z - Z^2) + C

540 -- F(Z) = LOG(1 / (COS(Z^2 + C)))

541 -- F(Z) = Z^3 + (TAN(Z) + C * Z)^2

542 -- F(Z) = Z^2 * X - Z * Y + C

543 -- F(Z) = Z^2 * CSC(Z^2) + C

544 -- F(Z) = (Z + LOG(Z))^3 + C

545 -- F(Z) = Z^(LOG(Z^2)) - Z + C

546 -- F(Z) = (2Z^4 - Z + C) / (Z + C)

547 -- F(Z) = Z^5C - Z^3C + Z^C + C

548 -- F(Z) = Z^2 + ((Z^3) / (TAN(Z)^2))) + C

549 -- F(Z) = C^(Z^2 - Z + C)

550 -- F(Z) = Z^7 + ((Z^5) / (5 - Z)) + ((Z^3) / (3 - Z)) + Z / C

551 -- F(Z) = (TAN(C * Z))^2 + C

552 -- F(Z) = Z^3 + (1 + LOG(Z))^2 + C

The next group of 55 equations are exhibited
in the 2006 "D" line of fractal imagery.

553 -- F(Z) = Z ^ (2 / SIN Z) + C

554 -- F(Z) = Z ^ (2 / TAN Z) + C

555 -- F(Z) = Z ^ (3 / COS Z) + C

556 -- F(Z) = Z ^ (3 / TAN Z) + C

557 -- F(Z) = Z ^ (2 / (1 + LN Z)) + C

558 -- F(Z) = Z ^ (3 / (1 + LN Z)) + C

559 -- F(Z) = Z ^ (2 / (ATAN Z) + C

560 -- F(Z) = Z ^ (3 / (ATAN Z) + C

561 -- F(Z) = (1 + Z ^ (2/Z)) ^ Z + C

562 -- F(Z) = (1 + Z ^ (2/(1-Z^2))) + C

563 -- F(Z) = (1 + Z ^ (2/(1-Z))) ^ 2 + C

564 -- F(Z) = (1 + Z ^ (2/(1-Z^2))) ^ 2 + C

565 -- F(Z) = (1 + Z ^ (2/(1-Z))) ^ Z + C

566 -- F(Z) = (1 + Z ^ (4/Z^2)) + C

567 -- F(Z) = (Z ^ 2 - z ^ (4/Z)) + C

568 -- F(Z) = (Z + ATAN(1 / Z)) ^ 2 + C

569 -- F(Z) = (Z + ATAN(1 / C)) ^ 2 + C

570 -- F(Z) = (1 + Z * ATAN(Z)) ^ 2 + C

571 -- F(Z) = (Z + C * ATAN(SQRT(Z))) ^ 2 + C

572 -- F(Z) = (Z + ATAN(1/Z)) ^ 3 + C

573 -- F(Z) = (Z + (1 / (ATAN(1/Z))) ^ 2 + C

574 -- F(Z) = (Z + (C / (ATAN(1/Z))) ^ 2

575 -- F(Z) = Z ^ 5 + (1 + ATAN(Z)) ^ 2 + C

576 -- F(Z) = Z ^ 4 + (1 - TAN(1/Z)) ^ 2 + C

577 -- F(Z) = Z ^ 3 + (C + 1/Z) ^ 2 + C

578 -- F(Z) = Z ^ 4 - 3X ^ 3 - 2Y ^ 2 - Z + C

579 -- F(Z) = (Z ^ 6 / (6Z ^ 5 + C) + C

580 -- F(Z) = ((Z ^ 6 + C )/ (5Z ^ 4)) + C

581 -- F(Z) = ((Z ^ 5 + C )/ (4Z ^ 3)) + C

582 -- F(Z) = ((Z ^ 4 + Z ^ 3) / (3Z ^ 2 + C)) + C

583 -- F(Z) = C / (Z ^ 2 * LN Z)

584 -- F(Z) = (1 / (Z ^ 2 * LN Z)) + C

585 -- F(Z) = 1/Z^4 - 1/Z^3 + 1/Z^2 - 1/Z + C

586 -- F(Z) = X^2 * SIN Z + Y^2 * COS Z + Z^2 + C

587 -- F(Z) = X^2 * Y^2 - Z^2 + Z + C

588 -- F(Z) = Z^2 + XYC^2 + C

589 -- F(Z) = Z^2 + ATAN(Z^2) + C

590 -- F(Z) = X^2*Y - X*Y^2 + Z + C

591 -- F(Z) = X^2*Y^2*Z^2 + ATAN Z + C

592 -- F(Z) = Z^2 + (ATAN (XYZ)) ^ 2 + C

593 -- F(Z) = (1 + LN(1 + Z)) ^ 2 + C

594 -- F(Z) = (Z^4 + C) / (ATAN Z)

595 -- F(Z) = (1 + (Z / ACOS Z)) ^ 2 + C

596 -- F(Z) = (1 + SQRT(Z^2 + ATAN Z)) ^ 2 + C

597 -- F(Z) = (Z^2 + SQRT(1 + (LN Z)^2)) ^ 2 + C

598 -- F(Z) = Z ^ (2 + ATAN Z + C)

599 -- F(Z) = C ^ (Z ^ 2 + (1 /(1 + LN Z))) + C

600 -- F(Z) = (1 + ATAN Z) ^ 2 + (1 + ATAN 2Z) ^ 2 + C

601 -- F(Z) = (1 + Z + ATAN 3Z) ^ 2 + C

602 -- F(Z) = (Z + ((1 + ATAN 2Z) ^ 2)) + C

603 -- F(Z) = (1 + ACOS Z) ^ 2 + C

604 -- F(Z) = (1 + XYZ) ^ 2 + C

605 -- F(Z) = Z^2 - X^2*Y*ACOS Z + C

606 -- F(Z) = Z^3 + XY^3 + X^2*Z^3 - YZ + C

607 -- F(Z) = Z^4 - YZ^3 + XZ^2 - ZC^2 + C

608 -- F(Z) = Z^(3/2) - (3/2)Z + Z^(1/2) + C

The next group of 71 equations are exhibited in the
brand new 2008 "W" line of fractal imagery.

609 -- F(Z) = (C / (1 - Z)) ^ 2 + C

610 -- F(Z) = ((Z^2 + 1) / ( 1 - Z)) ^ 2 + C

611 -- F(Z) = ((Z^3 - XY^2 + YZ + 1) / (1 - X - Y)) + C

612 -- F(Z) = ((Z^5 + CZ^3 - C^2*Z) / (1 + X^2 + Y^2 - Z)) + C

613 -- F(Z) = Z^(5/2)*X^(3/2)*Y^(1/2) + C

614 -- F(Z) = Z^3 + (1 - XY) ^ 2 + C

615 -- F(Z) = Z^4 + (1 + X) ^ 2 - (1 - Y) ^ 2 + C

616 -- F(Z) = (Z^7 + C) / (1 + X^3 - Y^3)

617 -- F(Z) = ((Z^6 + X + Y^3) / (1 - Z^2 + Y^2)) + C

618 -- F(Z) = ((XZ^4 - YZ^3 + C) / (1 + XZ - YZ^2)) + C

619 -- F(Z) = ((Z^5 - Z^3 + X^2 - Y) / (1 + CXY + Z^2)) + C

620 -- F(Z) = Z^(5/2) - Z^(3/2) + C^(3/2) + C

621 -- F(Z) = (1 + C + Z) ^ (5/2) + C

622 -- F(Z) = Z ^ (1 - Z^2) + C

623 -- F(Z) = Z ^ (Z - SIN Z) + C

624 -- F(Z) = Z ^ (1 + TAN Z) + C

625 -- F(Z) = Z ^ ((1 + LN Z) ^ 2) + C

626 -- F(Z) = e ^ ((Z + C)^2) + C

627 -- F(Z) = Z ^ (Z^2 / (1 - Z)) + C

628 -- F(Z) = Z ^ ((1 + TAN Z) ^ 2) + C

629 -- F(Z) = C ^ (Z + (1 + TAN Z)^2) + C

630 -- F(Z) = Z ^ ((Z^2 + SIN(1/Z))^2) + C

631 -- F(Z) = Z ^ (3 - Z) + Z ^ (1 + Z) + C

632 -- F(Z) = Z^2 COS X + Z + C

633 -- F(Z) = Z^3 * (COS X)^2 + Z^2 * SIN Y + C

634 -- F(Z) = Z^2 * ATAN C + C

635 -- F(Z) = Z^2 * ACOS Z + C

636 -- F(Z) = Z^2 + (1 - COS Z) ^ 2 + C

637 -- F(Z) = (e^Z - e^(-Z)) / C + C

638 -- F(Z) = Z^2 + SINH Z + C

639 -- F(Z) = (1 + Z + LN(1 + Z^2)) ^ 2 + C

640 -- F(Z) = (Z^2 / (Z + e^(1 - Z))) + c

641 -- F(Z) = ((Z^3 + 2 LN (1 + Z)) / e^Z) + C

642 -- F(Z) = (Z^12 - 12Z^11 - 11Z^10 - 10Z^9 + C) / (Z^4 + Z^2 + 1)

643 -- F(Z) = (Z^8 + Z^6 + Z^4 + Z^2 + 1) / (C^3 + C^2 + C + 1)

644 -- F(Z) = Z^7 - Z^5 - Z^3 + Z^2 + C

645 -- F(Z) = ((Z^5 - Z^4 + 1) / (Z^3 - Z + 1)) + C

646 -- F(Z) = ((Z^7 + Z^3 + C) / (Z^5 - C^2)) + C

647 -- F(Z) = e^(1 + SIN Z) - e^(2 - COS Z) + Z^(2 - C) + C

648 -- F(Z) = SQRT(Z^3 + Z^2) + C

649 -- F(Z) = SQRT(Z^4 + (1 + Z^2)^3) + C

650 -- F(Z) = SQRT(Z^5 + Z^3 + C) + C

651 -- F(Z) = SQRT(Z^4 + (1 + e^Z)^2) + C

652 -- F(Z) = SQRT(Z^6 + (1 + COS Z)^2) + C

653 -- F(Z) = SQRT(Z^4 + ATAN(X^2 + Y^2 + Z^2)) + C

654 -- F(Z) = SQRT(Z^6 + Z^4 + Z^2 + 1) + C

655 -- F(Z) = SQRT(Z^4 + e^(Z + SIN Z)) + C

656 -- F(Z) = SQRT(Z^3 + (1 + Z)^(5/2)) + C

657 -- F(Z) = CBRT(Z^7 + Z^5 * e^Z) + C

658 -- F(Z) = CBRT(e^(Z^2 + C)) + C

659 -- F(Z) = CBRT(Z^8 - Z^5 + 1) + C

660 -- F(Z) = CBRT(1 + ABS(ATAN(Z))^5 + Z^4) + C

661 -- F(Z) = CBRT(Z^6 - e^(2 - Z) + 1) + C

662 -- F(Z) = CBRT(e^(Z^2 * LN(ABS(1+Z))) + 1) + C

663 -- F(Z) = (Z^9 - Z^4 + 1) ^ (e^Z) + C

664 -- F(Z) = Z^(5/2) + (1 + SIN (Z/2)) ^ 2 + C

665 -- F(Z) = (1 + SIN(Z + COS Z)) ^ 2 + C

666 -- F(Z) = (Z ^ (2 / COS Z)) ^ 2 + C

667 -- F(Z) = e ^ (Z* (1 + COS Z)^2) + C

668 -- F(Z) = (e^2Z / (1 - Z)^2) + C

669 -- F(Z) = LN(1 + Z^2 + Z^4) + C

670 -- F(Z) = Z - Z^3/6 + Z^5/120 - Z^7/5040 + C

671 -- F(Z) = e ^ Z ^ (5/2) + C

672 -- F(Z) = (Z ^ 3 + ABS Z + 1) ^ Z + C

673 -- F(Z) = Z^2 / (COS Z * (1 + TAN Z)) + C

674 -- F(Z) = Z ^ (7/2) + (7/2) ^ Z + C

675 -- F(Z) = Z^6 + Z ^ (Z + 3) + C

676 -- F(Z) = e^Z * SIN Z + e^(-Z) * ( 1 + ATAN Z) + C

677 -- F(Z) = (1 + Z*e^(-Z)) ^ 2 + C

678 -- F(Z) = (Z^C / (1 + C)) + C

679 -- F(Z) = (Z^Z / (1 - Z)) + Z + C

1001 -- F1(Z) = Z^(10-Z) + Z + C; F2(Z) = (1+SIN(Z))^2 + C

1002 -- F1(Z) = Z^(11-Z^2) - Z + C; F2(Z) = (Z+TAN(Z))^2 + C

1003 -- F1(Z) = Z^12(1+SIN(Z)) - Z^2 + C; F2(Z) = Z^(1-Z^2) + C

1004 -- F1(Z) = Z^(2 + COS(Z)) + C; F2(Z) = Z^(12.5) + C

1005 -- F1(Z) = Z^12.5 + C; F2(Z) = Z^2.05 + C

1006 -- F1(Z) = 1 + SIN(Z^12) + C; F2(Z) = Z^2.5 - Z + C

1007 -- F1(Z) = Z^SQRT(12) + C; F2(Z) = Z^2*(1 + SIN(Z)) - Z + C

1008 -- F1(Z) = REAL(Z)*COS(C^2*Z^SQRT(12)) + C; F2(Z) = ATAN(Z^5) + Z^2 + C

1009 -- F1(Z) = 1 + SIN(Z^2 + Z^6 - Z^12) + C; F2(Z) = 1 + LOG(2/Z + Z + Z^2) + C

1010 -- F1(Z) = (Z + COS(Z))^6 - (Z - SIN(Z))^4 + C; F2(Z) = IMAG(Z^3) + Z^2 + 1 + C

1011 -- F1(Z) = (Z^12 - Z^9 + Z^6) / (Z^4 + 1) + C; F2(Z) = 1 + LOG(1 + REAL(Z^2) + COS(Z^3)) + C

1012 -- F1(Z) = (Z^12 + Z^8 + Z^4 + 1) / (Z^7 - 1) + C; F2(Z) = 1 + LOG(1 + REAL(Z^2) + COS(Z^3)) + C

1013 -- F1(Z) = (Z + COS(Z))^7 - (Z - COS(Z))^5 + C; F2(Z) = 1 + LOG(Z + COS(Z^3)) + C

1014 -- F1(Z) = (Z + SIN(Z))^7 - (SIN(REAL(Z)) - IMAG(Z))^5 + C; F2(Z) = Z^2 + REAL(Z^2 + 1 + COS(Z^2)) + C

1015 -- F1(Z) = (Z^2 + SIN(Z))^5 + (SIN(REAL(Z) - IMAG(Z))^3 + C; F2(Z) = Z^2 + C

1016 -- F1(Z) = (Z^3 + SIN(Z))^8 - (SIN(REAL(Z) - IMAG(Z))^6 + C; F2(Z) = Z^(2-Z) + C

1017 -- F1(Z) = (1 + TANH(Z))^4 - (SIN(Z) - IMAG(Z))^2 + C; F2(Z) = Z^(4-Z) + C

1018 -- F1(Z) = (Z^2 + TAN(Z))^5 - (REAL(Z) + COS(1-Z))^2 + C; F2(Z) = Z^2 + C

1019 -- F1(Z) = (Z^3 + SIN(1 - Z^2))^3 + (Z^2 + COS(1-Z))^2 + C; F2(Z) = C - COS(Z^2) + REAL(C)

1020 -- F1(Z) = Z^4 + Z^C^2 + C; F2(Z) = ATAN(Z^2) + COS(1 - Z^2) + C

1021 -- F1(Z) = Z^7 + Z^C^3 + C; F2(Z) = REAL(Z^2) + COS(1 - Z^2) + C

1022 -- F1(Z) = Z^5 + REAL(Z^(3-3COS(Z)) + C; F2(Z) = Z^2 + SIN(Z^2 + Z + 1) + C

1023 -- F1(Z) = Z^5 + REAL(Z^(3-3COS(Z)) + C; F2(Z) = Z^4 + ACOS(Z + SIN(Z^2 + Z + 1)) + C

1024 -- F1(Z) = Z^Z + Z^7 + C; F2(Z) = Z^3 + ATAN(Z^2 + SIN(Z^2 + Z + 2)) + C

1025 -- F1(Z) = Z^5 + Z^(2/Z) + C; F2(Z) = Z^3 + ACOS(Z^2+ SIN(Z^2 +REAL(Z) + 2)) + C

1026 -- F1(Z) = (Z^5 + Z^(2/Z) + C) / (Z^3 + ACOS(Z^2+ SIN(Z^2 +REAL(Z) + 2)) + C); F2(Z) = Z^2 + C

1027 -- F1(Z) = (Z^15 + Z^(8/Z) + C) / (ACOS(Z^3 + Z^2 +SIN(REAL(Z))) + C; F2(Z) = Z^2 + C

1028 -- F1(Z) = Z^11 + Z^(4/Z) + C; F2(Z) = Z^5 / (Z^3 - Z + IMAG(Z)) + C

1029 -- F1(Z) = Z^7 + Z^(5*COS(Z)) + C; F2(Z) = Z^7 / (Z^4 - Z^2 + REAL(Z)) + C

1030 -- F1(Z) = Z^9 + Z^(7*TAN(Z)) + C; F2(Z) = Z^6 / (Z^4 + Z^2 + IMAG(Z)) + C

1031 -- F1(Z) = Z^(3SIN(1-Z) + Z^6 + C; F2(Z) = (Z^5COS(Z) / (Z^3 - REAL(Z) + 1)) + C

1032 -- F1(Z) = Z^5(1-COS(Z)) + Z^8 + C; F2(Z) = (Z^7SIN(Z) / (Z^2 + IMAG(Z) + 1)) + C

1033 -- F1(Z) = Z^14(1-SIN(Z)) + Z^11.5 + C; F2(Z) = Z^5LOG(Z) / (Z^3 + IMAG(Z) - 1)) + C

1034 -- F1(Z) = Z^11.5SIN(1 - Z^5) + Z^5.5 + C; F2(Z) = Z^7LOG(2-Z) / (Z^4 + REAL(Z) - 1) + C

1035 -- F1(Z) = CZ^7.5*COS(Z) + C; F2(Z) = (1 + SQRT(Z) + LOG(Z))^9 + Z^4 + C
</pre>

# Fractal Noises
* https://github.com/tonysnail/Fractal-Wavetable-Generator
* https://github.com/hansel67/fractal-synth
* https://github.com/Adiaslow/Sound-Synthesizer-Python
* https://github.com/HackerPoet/FractalSoundExplorer
* https://github.com/mjdave/FluidNoise


# WaveShaper
* Generate wave shaper from fractalizer

# Methods
* noise + filters
* brownian noise + filters
* perlin noise + filters
