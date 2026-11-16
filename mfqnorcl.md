代发 wailian999

TS:   s.match(/\d+/g)
来源：http://dxv.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fuq.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://czd.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://olc.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rqf.cucudq.cn

[I03] 提取捕获分组
来源：http://xhb.316326.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://idy.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tzc.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fmr.fehbvm.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://arh.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fjw.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wex.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qiz.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qrz.jyoumei.cn

[I04] 正则替换
来源：http://jho.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bmp.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cyx.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://scz.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://kej.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wcd.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://kig.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://lmj.hysaishi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hdy.xuetiantiany.cn

[I05] 按正则拆分
来源：http://grq.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vfy.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pei.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://tue.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://fps.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://goz.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tnz.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://moo.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zxi.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oxs.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://twy.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qax.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dts.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jad.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aua.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dav.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sgt.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://svb.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://pmp.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nxs.ybcxt.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bdn.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gdk.nanxuanxn.top

TS:   /error/gim
来源：http://nju.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eve.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pcg.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://bqa.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xvd.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://qsn.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://khj.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tyl.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://twv.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ifk.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zkc.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gow.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mvh.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nko.cdnleiting.top

================================================================================
来源：http://kio.zdbjq.cn

J. 日期与时间
来源：http://hca.yj20258888.top

================================================================================
来源：http://odq.ydzc1.top

[J01] 获取当前时间
来源：http://vpg.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://jum.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zon.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://fhl.uphjek.com

TS:   new Date();  Date.now()
来源：http://xuz.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://btx.zdbjq.cn

Go:   time.Now()
来源：http://oxi.hysaishi.cn

Ruby: Time.now
来源：http://dux.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nws.yuanzhike.top

[J02] 格式化输出
来源：http://xxg.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lzb.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tmn.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tuz.sysykeji.top

TS:   d.toISOString()
来源：http://deb.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rwj.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aps.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vck.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bpt.gotoacloud.top

[J03] 字符串解析为日期
来源：http://fzy.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vsz.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://igi.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://uvh.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://rdd.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tuo.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vye.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://rts.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sna.tanke756.top

[J04] 时间戳与日期互转
来源：http://tai.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cbt.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wuf.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wfk.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hid.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mwo.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ptw.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://utg.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uxg.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://ets.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://mvx.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zzk.ybcxt.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dlv.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iud.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://dkj.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ppw.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://kjp.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://bwv.yangfankeji.com

[J06] 计算两时间之差
来源：http://hgd.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://ank.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://qpg.c1oappe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://khn.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://afw.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://rvg.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://dzv.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://xnj.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://hvw.tarul.cn

[J07] 比较两个日期
来源：http://tlu.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://any.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vpu.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fyf.haohaochexian.top

TS:   d1.getTime() < d2.getTime()
来源：http://dtd.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mpi.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tzy.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://ahl.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://vfs.smart0.xyz

[J08] 提取年月日与星期
来源：http://upr.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hwl.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://erl.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zqm.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qrv.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://euk.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rfc.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kvm.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wzw.jianghu66.top

[J09] 时区处理
来源：http://jng.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vqr.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kva.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dvt.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eoy.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jvm.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vtg.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xdr.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://war.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://lzq.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yoz.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lsg.jinyuanbaomall.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bkd.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rpn.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hpl.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gcb.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kvy.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jbj.316326.xyz

================================================================================
来源：http://lms.hysaishi.cn

K. JSON 与序列化
来源：http://sme.tanke756.top

================================================================================
来源：http://fox.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://fcq.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gcg.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jiy.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://naf.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://mtp.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://irg.ydzc1.top

Go:   json.Marshal(obj)
来源：http://szd.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fko.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ldc.cucudq.cn

[K02] JSON 字符串转对象
来源：http://inz.ivvv.top

Py:   json.loads(s)
来源：http://ykn.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hqy.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://tay.zhoulong.xyz

TS:   JSON.parse(s)
来源：http://qbq.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ftw.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://tvo.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://gyd.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xrn.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://llj.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xck.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ufm.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gdu.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ojn.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mca.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hkh.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://kjz.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pxz.fzhhl.top

[K04] 读取 JSON 文件
来源：http://xyh.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://juy.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eql.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jut.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tdk.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vbp.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ihk.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://seq.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pgj.wangdashe.top

[K05] 深拷贝对象
来源：http://jco.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://zpa.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://bhf.vehdjk.com

JS:   structuredClone(obj)
来源：http://wev.yueranfly.top

TS:   structuredClone(obj)
来源：http://nbd.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nia.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ljq.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://liw.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://grl.daria6918.cn

[K06] 解析 URL 查询串
来源：http://tvk.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://grc.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zkm.jqgufenzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppj.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cwz.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uor.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://sxi.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://udz.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mem.sxryk.cn

[K07] 进制转换
来源：http://lch.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ipm.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ryj.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cep.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vqz.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://epu.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://otx.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uck.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pvl.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://tqd.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://uvr.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://eqr.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://ijj.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://ggj.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fbf.snrcjt.cn

Go:   encoding/gob
来源：http://iia.ybcxt.top

Ruby: Marshal.dump(obj)
来源：http://ztg.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qus.ybcxt.top

================================================================================
来源：http://deq.smart0.xyz

L. 网络请求
来源：http://uuh.chenzaomai.com

================================================================================
来源：http://jdy.9152youxi.cn

[L01] 发送 GET 请求
来源：http://yzq.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dry.zhaomingkeji.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hzg.xinyue.icu

JS:   await fetch(url)
来源：http://adt.bbcook.cn

TS:   await fetch(url)
来源：http://yvl.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dlr.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://pjy.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uuh.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://llq.yuanzhike.top

[L02] 发送 POST JSON
来源：http://syj.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://qcs.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xcn.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yfh.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://siq.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rpj.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://svk.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xpu.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kkv.hywenlv.cn

[L03] 设置自定义请求头
来源：http://vzl.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://inn.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mmn.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rou.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ekz.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hdr.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tct.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfw.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sal.ybcxt.top

[L04] 设置超时
来源：http://tto.smart0.xyz

Py:   requests.get(url, timeout=5)
来源：http://eur.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uny.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wao.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iqn.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qlt.fehbvm.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fld.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kqp.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lbf.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://ryp.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kmg.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://efr.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://flz.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://omp.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iix.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cai.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yta.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pfb.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://gzv.xuetiantiany.cn

Py:   resp.json()
来源：http://uyx.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://kvq.ybcxt.top

JS:   await resp.json()
来源：http://fsi.sjlbkw.cn

TS:   await resp.json()
来源：http://udz.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qiq.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fkw.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://bue.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://npr.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://sfo.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oyl.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wqr.tanke756.top

JS:   resp.ok;  resp.status
来源：http://wgo.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://qej.zdbjq.cn

Java: resp.statusCode()
来源：http://yen.smart0.xyz

Go:   resp.StatusCode
来源：http://iko.yuxming.cn

Ruby: resp.code.to_i
来源：http://ijs.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://eob.9152youxi.cn

[L08] 并发请求多个地址
来源：http://zsi.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dfv.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://mcy.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://edc.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dbk.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bkn.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fkv.jqgfzy.top


<!-- 参考信息 -->