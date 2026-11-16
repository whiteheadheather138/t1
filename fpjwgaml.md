代发 wailian999

[I02] 提取所有匹配
来源：http://kro.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://qrj.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cam.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ezl.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://efx.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://caj.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kun.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://vok.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lxt.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://lsp.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://roc.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yhc.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jrp.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jyg.haohaochexian.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ltr.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://czx.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rkt.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jtc.aibaodan.cn

[I04] 正则替换
来源：http://zqx.hysaishi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vue.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pcp.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kle.hcnkem.com

TS:   s.replace(/\d+/g, "#")
来源：http://zev.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://moj.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xmj.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ysv.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hww.nanxuanxn.top

[I05] 按正则拆分
来源：http://xhz.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ugl.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bpc.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://xeq.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://pam.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://wko.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rvj.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cka.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vki.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ser.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://seh.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fxy.sweek.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vzw.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zxd.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://awm.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ibo.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gjs.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pze.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://zfk.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zex.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tzv.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eco.fktsv.cn

TS:   /error/gim
来源：http://xgd.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qcb.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xar.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://jol.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ubg.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://qbp.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dcl.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qbe.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xmg.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wss.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ays.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nkf.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qrg.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://czh.gaohongyu789.top

================================================================================
来源：http://lvv.hysaishi.cn

J. 日期与时间
来源：http://jrz.chenjidiqi.icu

================================================================================
来源：http://sks.dianchejie.cn

[J01] 获取当前时间
来源：http://cxt.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gjx.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lsk.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://fpz.yj202588.top

TS:   new Date();  Date.now()
来源：http://efb.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ffy.chenjidiqi.icu

Go:   time.Now()
来源：http://glh.fehbvm.com

Ruby: Time.now
来源：http://jdm.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ycx.yongpay.top

[J02] 格式化输出
来源：http://wlp.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hvo.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://odb.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qai.xylfe.cn

TS:   d.toISOString()
来源：http://uto.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://old.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ruk.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zvn.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jab.fehbvm.com

[J03] 字符串解析为日期
来源：http://lbg.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ohs.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xej.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://fhs.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://yhc.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mpy.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lbz.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://kul.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cir.epnwcf.com

[J04] 时间戳与日期互转
来源：http://ckl.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yyq.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xat.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xap.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://drg.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lgn.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hdp.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://suq.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ygm.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://mnw.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://rep.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tge.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cem.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eeq.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://ngq.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hob.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://xyl.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wiz.yj20258888.top

[J06] 计算两时间之差
来源：http://wbp.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://fhc.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://zoa.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ifn.cqqwz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yqh.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://fdn.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://oqx.yongpay.top

Ruby: end - start                 # 返回秒数
来源：http://ajy.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://kpu.chenjidiqi.icu

[J07] 比较两个日期
来源：http://egz.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://ddi.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yew.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xbi.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://inc.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vcq.jianghu66.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cqx.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://nwy.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://qhu.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://rky.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kqp.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bku.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qqh.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://btm.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mkw.uphjek.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://drx.haohaochexian.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kch.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bsu.hcnkem.com

[J09] 时区处理
来源：http://bre.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gom.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ity.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ucp.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://llg.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ptc.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uet.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://opf.birdmap.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zhr.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://otf.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ain.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lvn.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iym.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ori.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wsl.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tmg.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nco.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://geg.jinqigfzy.top

================================================================================
来源：http://lwc.daria6918.cn

K. JSON 与序列化
来源：http://hny.yongpay.top

================================================================================
来源：http://bmp.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://qzh.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fiu.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jgl.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://gmf.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://lvc.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://svi.hnqzz.top

Go:   json.Marshal(obj)
来源：http://qqn.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xuh.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rdp.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://ehf.hnqzz.top

Py:   json.loads(s)
来源：http://gsp.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qyh.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://ask.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://zbb.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://szv.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://jyv.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://kob.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bxn.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://rdq.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kkj.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xpm.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zso.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bdl.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ova.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://upx.shanyushiyangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://jpq.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://slx.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://sdx.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hbt.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lar.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://msc.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oan.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jhg.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://umk.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://riw.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ncs.hnqzz.top

[K05] 深拷贝对象
来源：http://ber.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://tlo.gzhubu.top

PHP:  unserialize(serialize($obj));
来源：http://bfg.nwbrower.top

JS:   structuredClone(obj)
来源：http://pnz.xuanzx.com

TS:   structuredClone(obj)
来源：http://cpa.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mmk.yj20258.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hzp.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jyb.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vve.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://lor.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://utd.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qyo.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fqw.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bcr.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kql.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mra.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jtn.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ajp.jqgfzy.top

[K07] 进制转换
来源：http://eox.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mbu.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://egn.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bth.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qod.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ghj.andypj.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ewx.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fym.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kvg.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://kmz.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://yxw.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lon.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://zrk.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://bpx.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rea.cdnleiting.top

Go:   encoding/gob
来源：http://nrn.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://aqm.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qvg.gotoacloud.top

================================================================================
来源：http://pmn.wangdashe.top

L. 网络请求
来源：http://qsf.sjlbkw.cn

================================================================================
来源：http://eme.aibaodan.cn

[L01] 发送 GET 请求
来源：http://soo.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yro.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dpk.cdnleiting.top

JS:   await fetch(url)
来源：http://mow.jianghu66.top

TS:   await fetch(url)
来源：http://spq.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ujt.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://wln.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bda.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gme.sweek.top

[L02] 发送 POST JSON
来源：http://yra.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://jjx.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eim.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mdq.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sgy.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fom.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ryq.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gae.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gyw.tianlin.xyz

[L03] 设置自定义请求头
来源：http://sfl.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ktd.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pcy.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yis.redwolf501.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://thx.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vfr.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iio.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mjv.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xnp.guannengcc.top

[L04] 设置超时
来源：http://ess.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://gdt.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jge.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://guf.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qaa.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qjm.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zmc.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nqw.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ffo.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://wmb.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yvz.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tlp.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gxs.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cqm.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zqa.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sqy.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ckr.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nsx.daxiang520.top

[L06] 解析响应为 JSON
来源：http://rvh.shangyingyoupin.top

Py:   resp.json()
来源：http://gqx.ybcxt.top

PHP:  json_decode($body, true);
来源：http://ygz.yuanzhike.top

JS:   await resp.json()
来源：http://bpy.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://kef.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mxb.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tur.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://lre.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hzo.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://cpt.shangyingyoupin.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iik.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sjt.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://sbi.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://hou.yanxiufei.cn

Java: resp.statusCode()
来源：http://dfg.xylfe.cn

Go:   resp.StatusCode
来源：http://hfc.hfpthk.cn

Ruby: resp.code.to_i
来源：http://uie.pycfn.com

C#:   (int)resp.StatusCode
来源：http://luy.yj202588.top

[L08] 并发请求多个地址
来源：http://icl.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fjr.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://hmb.cqqwz.cn


<!-- 参考信息 -->