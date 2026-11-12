代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dpi.cashguo.top

PHP:  preg_match('/\d+/', $s);
来源：http://jgr.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://nwp.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://ffz.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lil.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ets.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://hrz.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dyz.fehbvm.com

[I02] 提取所有匹配
来源：http://dya.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://nsf.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://byg.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://odw.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://fai.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jje.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aby.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://bxn.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yag.tanke756.top

[I03] 提取捕获分组
来源：http://ejf.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tas.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://azx.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jiv.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tjp.fanxiaobao.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xtd.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fxz.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zrz.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vxu.jlsjyb.cn

[I04] 正则替换
来源：http://zwe.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fxx.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sox.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://ywl.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://iou.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://fph.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tox.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sgh.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ksz.xingfuxueyuan.xyz

[I05] 按正则拆分
来源：http://xor.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://shi.yongpay.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://swu.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://drq.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://rnq.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://opr.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://abr.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://khx.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dgx.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uyv.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bav.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wdk.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nxy.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://muc.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yjb.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tpz.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wuf.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bmj.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://ayo.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vnw.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kqm.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jth.redwolf501.top

TS:   /error/gim
来源：http://elo.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://isx.nwbrower.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bke.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://dse.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://epn.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://jkq.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gcm.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://msu.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uoo.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ahk.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sor.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vkt.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://czl.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pss.hesvh.cn

================================================================================
来源：http://xvt.zhijiandao.cn

J. 日期与时间
来源：http://rrl.ehwqpu.com

================================================================================
来源：http://bud.zhijiandao.cn

[J01] 获取当前时间
来源：http://xbc.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lzx.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pzv.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://uvq.yuanzhike.top

TS:   new Date();  Date.now()
来源：http://vuy.bjfxy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uqo.yj202588.top

Go:   time.Now()
来源：http://rmn.cucudq.cn

Ruby: Time.now
来源：http://med.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hoo.yongpay.top

[J02] 格式化输出
来源：http://mwk.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xks.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iqi.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bzn.feifeiyinyue.top

TS:   d.toISOString()
来源：http://fdf.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nig.52xcode.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nrq.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vml.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ato.andypj.xyz

[J03] 字符串解析为日期
来源：http://qlh.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mvt.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nfi.hammf.cn

JS:   new Date("2024-01-02")
来源：http://ioz.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://gle.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://apk.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hvy.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://tvg.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cqe.tanke756.top

[J04] 时间戳与日期互转
来源：http://ujh.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wor.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rlb.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mdz.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://yrf.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rdu.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lch.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lox.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rdw.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://vjm.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://atd.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ssf.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xkn.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ddw.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://syd.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://spp.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://mbf.wangdashe.top

C#:   DateTime.Now.AddDays(7)
来源：http://ipl.iojbl.cn

[J06] 计算两时间之差
来源：http://iva.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://oqx.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://wjb.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://crv.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wik.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://fck.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://mmy.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://ykd.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://adv.hysaishi.cn

[J07] 比较两个日期
来源：http://koz.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://ltc.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pqh.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rrs.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://tht.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rvx.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ynf.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://zvt.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://zcz.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://ryp.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tso.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mpb.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oup.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jkp.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qfo.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tua.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fue.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rpj.gzhubu.top

[J09] 时区处理
来源：http://mkw.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hqa.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fpx.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://syb.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fhz.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ndk.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rxe.52xcode.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ery.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bvm.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://jgu.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://wys.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tub.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xdh.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fpk.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xof.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://shq.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kzx.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tkj.ydzc1.top

================================================================================
来源：http://jpn.sjlbkw.cn

K. JSON 与序列化
来源：http://sqj.jinqigfzy.top

================================================================================
来源：http://xcc.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://imn.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bem.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hse.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://ddy.cheryme.top

TS:   JSON.stringify(obj)
来源：http://bbc.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ebn.meibo888.top

Go:   json.Marshal(obj)
来源：http://xqi.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://xnq.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hmk.nwbrower.top

[K02] JSON 字符串转对象
来源：http://xqh.ctjpmb.com

Py:   json.loads(s)
来源：http://quu.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mxe.yongpay.top

JS:   JSON.parse(s)
来源：http://iol.yonumen.top

TS:   JSON.parse(s)
来源：http://yun.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ypz.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://mnf.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://bke.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ppa.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://lgx.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://icr.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nax.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sdo.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cga.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zwq.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://huf.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mlt.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tdg.daria6918.cn

[K04] 读取 JSON 文件
来源：http://jcy.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dcc.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zkj.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dre.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvg.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mzr.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pbo.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hdt.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xao.ehwqpu.com

[K05] 深拷贝对象
来源：http://owr.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://cfl.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://bes.yangfankeji.com

JS:   structuredClone(obj)
来源：http://aqp.jiagoushi.top

TS:   structuredClone(obj)
来源：http://afm.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://via.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fci.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mcf.dianchejie.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ses.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://xvm.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cda.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tsz.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bbf.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fbn.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://afc.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://lcv.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bpq.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uzx.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://jrn.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ryq.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vqm.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ncx.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://roy.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://djs.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hre.chenzaomai.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gnk.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nry.jinghuilouyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://gzj.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://jmj.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://wxs.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://cmj.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://wmh.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gcq.nanxuanxn.top

Go:   encoding/gob
来源：http://vjo.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://ydn.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bcr.fzhhl.top

================================================================================
来源：http://esc.nwbrower.top

L. 网络请求
来源：http://xvy.wangshuangyany.cn

================================================================================
来源：http://pdv.hysaishi.cn

[L01] 发送 GET 请求
来源：http://dut.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nkf.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kvl.ydzc1.top

JS:   await fetch(url)
来源：http://upa.feifeiyinyue.top

TS:   await fetch(url)
来源：http://gug.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wjn.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://elo.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qaw.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://you.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://zdb.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://jbo.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jlu.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lgo.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qig.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mew.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nht.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jds.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mgi.aibaodan.cn

[L03] 设置自定义请求头
来源：http://zke.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xvv.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://anp.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://irp.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://msy.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ssf.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dqx.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fnq.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mrp.shuidangran.top

[L04] 设置超时
来源：http://njm.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://kyk.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hos.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wnz.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zzl.chenjidiqi.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jvs.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ytt.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://icy.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tgp.yonumen.top

[L05] 上传文件（multipart）
来源：http://lxd.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nht.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://emf.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pcq.jinghuilouyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zqy.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kdy.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dfr.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://noj.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wcj.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://nks.52xcode.cn

Py:   resp.json()
来源：http://esm.epnwcf.com

PHP:  json_decode($body, true);
来源：http://vga.yangfankeji.com

JS:   await resp.json()
来源：http://ads.52xcode.cn

TS:   await resp.json()
来源：http://ret.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qld.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://glv.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://xmu.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kgu.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://opv.havefunace.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://itf.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://git.gogol.net.cn

JS:   resp.ok;  resp.status
来源：http://bms.zhijiandao.cn


<!-- 参考信息 -->