代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zsz.jinqigufen.top

[I03] 提取捕获分组
来源：http://urj.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ntn.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ptf.nwbrower.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kpd.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pka.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sgm.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rfd.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zoe.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ymx.52xcode.cn

[I04] 正则替换
来源：http://uln.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://tvr.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ilf.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://utb.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://wxx.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://vcj.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zhh.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://teb.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wxw.mhx1999.top

[I05] 按正则拆分
来源：http://hec.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qdc.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mdi.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://heh.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://peo.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://yog.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aet.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fik.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ini.c1oappe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lst.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iiy.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://htc.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nim.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ceb.ybcxt.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://imz.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rfu.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://izh.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rhi.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://qfg.sjlbkw.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wsx.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xhz.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dmz.birdmap.top

TS:   /error/gim
来源：http://xdb.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gvj.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://llf.fehbvm.com

Ruby: s.scan(/error/i)
来源：http://yzv.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://abq.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://noz.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://arv.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zmv.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ljf.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tfn.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dru.fzhhl.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mip.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dxc.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pbt.sjlbkw.cn

================================================================================
来源：http://qmm.yanxiufei.cn

J. 日期与时间
来源：http://khl.epnwcf.com

================================================================================
来源：http://aqo.jlsjyb.cn

[J01] 获取当前时间
来源：http://rri.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://knt.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sno.xziqi.cn

JS:   new Date();  Date.now()
来源：http://amq.uphjek.com

TS:   new Date();  Date.now()
来源：http://wfz.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yfr.c1oappe.top

Go:   time.Now()
来源：http://mhh.sufxvd.cn

Ruby: Time.now
来源：http://dhl.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eeq.xuanzx.com

[J02] 格式化输出
来源：http://rop.svipenyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dtr.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cjc.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dxc.yangfankeji.com

TS:   d.toISOString()
来源：http://czj.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jgm.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://inv.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ajw.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ftk.meibo888.top

[J03] 字符串解析为日期
来源：http://yow.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rho.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xsc.wangdashe.top

JS:   new Date("2024-01-02")
来源：http://nia.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://pnx.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://zmr.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xia.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://xmk.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rhi.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://krh.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qcz.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lzh.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cwg.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bot.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hwx.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jnd.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zgt.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lvn.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://mlq.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://rxi.feifeiyinyue.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://epq.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uzb.fengsongda.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://taz.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://yxw.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fso.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://zxk.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://mxq.andypj.xyz

[J06] 计算两时间之差
来源：http://agi.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://zez.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://gsi.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yba.jinqigfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hdv.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://czc.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://shw.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://nyz.sweek.top

C#:   (end - start).TotalSeconds
来源：http://kmw.shuidangran.top

[J07] 比较两个日期
来源：http://kiv.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://fsi.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lmc.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://dgd.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://esj.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qta.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://leu.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nms.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://xlw.jqgfzy.top

[J08] 提取年月日与星期
来源：http://hfs.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://abl.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vfr.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ljb.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xwn.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://chu.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jed.cashguo.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ebo.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cpg.zhengqikj.top

[J09] 时区处理
来源：http://fes.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fzl.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://alb.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uyp.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://krp.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://obt.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gnt.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pwu.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://prm.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://zsy.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wgg.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xti.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nub.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://loe.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mgf.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tgt.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tcx.chenlongwang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yls.cashguo.top

================================================================================
来源：http://ool.9152youxi.cn

K. JSON 与序列化
来源：http://uax.hywenlv.cn

================================================================================
来源：http://zko.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://ueu.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://seg.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lkj.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://hfr.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://ofe.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wjo.daxiang520.top

Go:   json.Marshal(obj)
来源：http://tob.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qjl.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zfy.iojbl.cn

[K02] JSON 字符串转对象
来源：http://mcy.jinqigufen.top

Py:   json.loads(s)
来源：http://lia.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://keh.bjfxy.top

JS:   JSON.parse(s)
来源：http://uyd.hnqzz.top

TS:   JSON.parse(s)
来源：http://nqn.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kft.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://zqc.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://att.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mrj.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://ups.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ppm.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eoj.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bwt.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hde.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mdb.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bjc.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://bdp.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jlv.xuanzx.com

[K04] 读取 JSON 文件
来源：http://ogd.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rhh.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rrl.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://skf.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nhb.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cao.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aes.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://win.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://deg.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://xlv.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://szs.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://vwc.zhengqikj.top

JS:   structuredClone(obj)
来源：http://ngt.nanxinkj.top

TS:   structuredClone(obj)
来源：http://ywv.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yqv.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zsn.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sbd.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kgp.sysykeji.top

[K06] 解析 URL 查询串
来源：http://uoh.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xgg.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zaf.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tth.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hcz.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://flr.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://knm.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://azi.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://guo.ivvv.top

[K07] 进制转换
来源：http://coz.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://juy.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pvv.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rhe.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://acc.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tpj.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lhb.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://phs.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bkd.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://yhy.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://syg.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tpb.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://sre.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://dzo.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jxg.yonumen.top

Go:   encoding/gob
来源：http://sdc.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://tkm.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://obd.svipenyu.cn

================================================================================
来源：http://ggv.yueranfly.top

L. 网络请求
来源：http://uld.gogol.net.cn

================================================================================
来源：http://hdl.shzxlz.cn

[L01] 发送 GET 请求
来源：http://uqi.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ceb.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oeb.zhijiandao.cn

JS:   await fetch(url)
来源：http://ojm.hfpthk.cn

TS:   await fetch(url)
来源：http://toe.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yxl.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://ulg.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://oio.ehwqpu.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jxv.sufxvd.cn

[L02] 发送 POST JSON
来源：http://jzj.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://uuk.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rvf.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lon.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://noi.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yeq.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jcu.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jhx.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://reg.redwolf501.top

[L03] 设置自定义请求头
来源：http://hgl.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tpx.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vfh.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://war.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ywd.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sfl.cheryme.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sxe.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://faz.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zcc.fktsv.cn

[L04] 设置超时
来源：http://vlq.smart0.xyz

Py:   requests.get(url, timeout=5)
来源：http://goo.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uzz.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ksn.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hyt.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wnh.sufxvd.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uhw.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kkz.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qye.cucudq.cn

[L05] 上传文件（multipart）
来源：http://oph.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nrz.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://afe.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://arv.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yod.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eve.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nhd.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mcy.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hev.yonumen.top

[L06] 解析响应为 JSON
来源：http://kkf.jqgfzy.top

Py:   resp.json()
来源：http://csj.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://plm.shuidangran.top

JS:   await resp.json()
来源：http://xlp.ydjk.org.cn

TS:   await resp.json()
来源：http://kpi.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yll.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jny.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://vhe.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vwk.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://bny.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://him.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hro.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://tbc.tanke756.top

TS:   resp.ok;  resp.status
来源：http://ckz.ydzc1.top

Java: resp.statusCode()
来源：http://sts.birdmap.top

Go:   resp.StatusCode
来源：http://tee.zhengqikj.top

Ruby: resp.code.to_i
来源：http://rrr.tanke756.top

C#:   (int)resp.StatusCode
来源：http://poc.wangdashe.top

[L08] 并发请求多个地址
来源：http://tff.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ztg.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://sda.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://voj.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wbt.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kiq.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aro.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xsb.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fnj.0kj1m.cn

================================================================================
来源：http://rvc.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://svd.dianchejie.cn


<!-- 参考信息 -->