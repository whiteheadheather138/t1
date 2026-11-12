代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://usq.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://feo.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://hdt.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://obu.smart0.xyz

[I02] 提取所有匹配
来源：http://ijo.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://rxn.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zzc.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mny.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://fxq.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ddy.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jxa.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://qog.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ncb.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://xmw.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qcj.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cvo.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ell.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zoq.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://okb.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hjo.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wwr.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xvz.gogol.net.cn

[I04] 正则替换
来源：http://mos.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ojj.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bgd.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://myr.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://qcl.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://hwf.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wfv.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pgn.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rlo.iojbl.cn

[I05] 按正则拆分
来源：http://yge.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zao.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://amw.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://lwj.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://lit.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://pnx.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://szc.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dzn.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yeg.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dfy.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nrv.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wov.sysykeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ikf.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mtd.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pty.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ydw.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mng.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iwz.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://cgk.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dxi.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://akx.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qyf.meibo888.top

TS:   /error/gim
来源：http://pno.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xfv.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dru.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://gjx.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eao.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://rjl.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jvh.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://esz.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ojz.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ezl.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://dvn.zycfv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ahx.hammf.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qhf.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://txz.fengsongda.top

================================================================================
来源：http://eyk.ywan-chungtsiang.top

J. 日期与时间
来源：http://nsh.316326.xyz

================================================================================
来源：http://fmc.yueranfly.top

[J01] 获取当前时间
来源：http://ery.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cit.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gag.fengsongda.top

JS:   new Date();  Date.now()
来源：http://llw.ydzc1.top

TS:   new Date();  Date.now()
来源：http://obc.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ine.gzhubu.top

Go:   time.Now()
来源：http://arg.ctjpmb.com

Ruby: Time.now
来源：http://zlc.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hfp.smart0.xyz

[J02] 格式化输出
来源：http://yza.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qxl.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vqk.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://glm.yj20258888.top

TS:   d.toISOString()
来源：http://ocr.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fzj.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uzf.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nsb.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ifp.jiagoushi.top

[J03] 字符串解析为日期
来源：http://xxb.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nxw.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uhr.uphjek.com

JS:   new Date("2024-01-02")
来源：http://zja.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://gtc.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gnq.sjlbkw.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bme.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://pme.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sjj.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://izv.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vtl.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://chh.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://swc.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dks.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ywc.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iqj.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bbw.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ylb.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://bbc.jinqigfzy.top

Py:   now + timedelta(days=7)
来源：http://com.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rzj.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vuf.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xdi.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://pyd.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hni.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://asu.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jqc.jiagoushi.top

[J06] 计算两时间之差
来源：http://zmg.yongpay.top

Py:   (end - start).total_seconds()
来源：http://kph.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://oyj.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://czi.gaohongyu789.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gsa.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://emq.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://hud.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://gob.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://tsf.kuanghao11.cn

[J07] 比较两个日期
来源：http://xnf.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://eno.zhoulong.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kde.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://iew.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xez.iojbl.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sda.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pyi.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fxw.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://rri.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://lel.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://top.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://udp.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ejb.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bgm.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zom.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lfy.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lny.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uux.9152youxi.cn

[J09] 时区处理
来源：http://vuu.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nit.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fxm.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fpq.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zkm.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ylz.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jgf.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cfr.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jah.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://yxe.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hgb.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://llf.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mym.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://akh.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://boc.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gvu.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vfu.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zcg.sjlbkw.cn

================================================================================
来源：http://upw.uphjek.com

K. JSON 与序列化
来源：http://ofs.yj20258888.top

================================================================================
来源：http://ujd.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://gqq.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jaf.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yyh.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://vfi.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://use.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vqn.guannengcc.top

Go:   json.Marshal(obj)
来源：http://ril.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://rco.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://rog.meibo888.top

[K02] JSON 字符串转对象
来源：http://ahq.chenlongwang.top

Py:   json.loads(s)
来源：http://krq.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://axy.daxiang520.top

JS:   JSON.parse(s)
来源：http://vgn.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://ele.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qod.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://dfo.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://sqn.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ewj.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://mtd.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oxv.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jge.chenjidiqi.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://bht.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ldp.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dxp.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qdm.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://vqo.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yzi.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://wqs.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rkm.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hns.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dgo.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yyu.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xmm.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hqs.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://akw.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uez.pycfn.com

[K05] 深拷贝对象
来源：http://dck.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://pft.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://wpw.hesvh.cn

JS:   structuredClone(obj)
来源：http://mgk.nanxinkj.top

TS:   structuredClone(obj)
来源：http://rel.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nrs.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qck.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jvv.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sbw.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://mgw.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vus.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://enp.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vvp.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kms.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dor.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ofn.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wso.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hpu.xuetiantiany.cn

[K07] 进制转换
来源：http://nxe.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yrv.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tfc.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yid.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://njl.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tru.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qdv.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tke.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gai.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://fsn.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://trc.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://smr.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://fxw.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://fes.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gib.bjfxy.top

Go:   encoding/gob
来源：http://uqq.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://kzv.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://okk.yueranfly.top

================================================================================
来源：http://tjr.sjlbkw.cn

L. 网络请求
来源：http://hau.yonumen.top

================================================================================
来源：http://tnw.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://adc.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oax.pycfn.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gcq.chenlongwang.top

JS:   await fetch(url)
来源：http://ilu.zhengqikj.top

TS:   await fetch(url)
来源：http://nzn.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oud.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://iwb.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sge.zhijiandao.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blz.svipenyu.cn

[L02] 发送 POST JSON
来源：http://asb.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rox.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ttd.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vum.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yen.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mzw.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xkk.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pnv.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tfg.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://qdd.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dxn.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bgy.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aib.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://srd.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ybe.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tyj.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tll.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vme.cdnleiting.top

[L04] 设置超时
来源：http://num.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://uyb.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vsd.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cwm.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://roz.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jlp.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://opp.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qvk.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fiy.aizwys.cn

[L05] 上传文件（multipart）
来源：http://zpm.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fvb.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wfz.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lby.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mzf.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rjx.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://glf.xuanzx.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ahp.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xzh.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://skx.cheryme.top

Py:   resp.json()
来源：http://tpi.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://urt.zhijiandao.cn

JS:   await resp.json()
来源：http://uuq.tianlin.xyz

TS:   await resp.json()
来源：http://adu.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iee.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://djj.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://rhw.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qvw.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://oja.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vmf.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://voh.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://zle.yj20258.top

TS:   resp.ok;  resp.status
来源：http://gnl.aizwys.cn

Java: resp.statusCode()
来源：http://ybo.cqqwz.cn

Go:   resp.StatusCode
来源：http://uah.zdbjq.cn

Ruby: resp.code.to_i
来源：http://abe.cqqwz.cn


<!-- 参考信息 -->