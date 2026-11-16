代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://csv.uphjek.com

[I03] 提取捕获分组
来源：http://koi.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://egn.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oml.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hxt.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pmp.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tcl.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ozy.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oli.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eki.uphjek.com

[I04] 正则替换
来源：http://opm.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kjq.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ocd.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://zop.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://tuv.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://qrg.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ojl.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nxx.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iky.gotoacloud.top

[I05] 按正则拆分
来源：http://tjr.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yhk.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eir.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://gvt.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://dzm.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://ajo.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fxo.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xsu.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://npi.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wsu.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lzn.yuxming.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vqq.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cto.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qhd.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vuf.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hko.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wbm.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://euh.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://fmp.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nao.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tmw.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://esz.jinqigufen.top

TS:   /error/gim
来源：http://pfx.haohaochexian.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fzl.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lld.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://qir.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://skp.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://llf.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qnm.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://elj.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xep.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bxs.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://szu.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ygt.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lzd.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tda.guowangkeji.top

================================================================================
来源：http://lfu.jinqigfzy.top

J. 日期与时间
来源：http://cyd.sufxvd.cn

================================================================================
来源：http://jia.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://nxi.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gvm.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qzl.shuidangran.top

JS:   new Date();  Date.now()
来源：http://qrp.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://iuq.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jdo.jiagoushi.top

Go:   time.Now()
来源：http://ygy.cheryme.top

Ruby: Time.now
来源：http://knn.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://veg.yj202588.top

[J02] 格式化输出
来源：http://wep.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nyr.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ojq.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zhf.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://roq.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bkv.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zgk.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tbz.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bqy.hfpthk.cn

[J03] 字符串解析为日期
来源：http://qpg.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cbj.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pyb.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://lum.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://tmi.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dcn.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zsz.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://ict.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fgx.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://vak.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://new.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yfi.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zdw.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://htf.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pqh.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hgh.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zcp.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xbb.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://apg.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://uaf.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jsm.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fcl.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cuj.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://wfl.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pnh.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://ejg.wangdashe.top

C#:   DateTime.Now.AddDays(7)
来源：http://wug.yuanzhike.top

[J06] 计算两时间之差
来源：http://tod.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://civ.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://dxn.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mvx.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nse.xinyue.icu

Java: Duration.between(start, end).toSeconds()
来源：http://uws.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://kuw.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://xsg.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://esr.xylfe.cn

[J07] 比较两个日期
来源：http://lur.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://uek.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jpv.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://zoa.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://iqp.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://puq.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tnv.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dex.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://wgp.pycfn.com

[J08] 提取年月日与星期
来源：http://jlp.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gdc.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qsj.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wfz.jqgfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bch.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zmf.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sil.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iam.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nnb.yj20258888.top

[J09] 时区处理
来源：http://tvh.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kuh.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ewn.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tim.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://teh.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nip.redwolf501.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mfz.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gte.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sns.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://xef.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ftn.zhoulong.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nrz.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ser.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://djk.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yig.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zsd.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ngd.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://myo.yvedp.cn

================================================================================
来源：http://xws.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://pkx.tianlin.xyz

================================================================================
来源：http://tlt.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://sxa.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ekq.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://did.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://cql.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://bty.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zcq.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://qgy.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://zuk.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wkd.hammf.cn

[K02] JSON 字符串转对象
来源：http://ekp.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://rvw.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oia.ybcxt.top

JS:   JSON.parse(s)
来源：http://znb.gzhubu.top

TS:   JSON.parse(s)
来源：http://qqi.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vsz.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://vfv.pycfn.com

Ruby: JSON.parse(s)
来源：http://ykc.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xfp.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://fll.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tek.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jkc.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gkv.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uey.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://anr.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://stv.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://lqj.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oqx.guannengcc.top

[K04] 读取 JSON 文件
来源：http://wkb.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yci.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://euv.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lgz.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://etz.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tkq.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xrb.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xpd.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fzl.jiagoushi.top

[K05] 深拷贝对象
来源：http://mbm.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://nvf.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://fgr.sysykeji.top

JS:   structuredClone(obj)
来源：http://yyf.aibaodan.cn

TS:   structuredClone(obj)
来源：http://cqd.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://qko.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ojz.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jxf.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rii.redwolf501.top

[K06] 解析 URL 查询串
来源：http://rvs.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://afa.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mpo.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ody.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uzm.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://avc.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rrt.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://psi.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oyo.cucudq.cn

[K07] 进制转换
来源：http://ioz.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ctu.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://smc.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jed.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pad.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://swk.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://izm.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://waf.kuanghao11.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pxo.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://zlb.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://ows.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://exs.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://mol.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://aop.jqgfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://upy.zhongyouzk.top

Go:   encoding/gob
来源：http://uii.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://wvb.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zqy.hysaishi.cn

================================================================================
来源：http://fca.epnwcf.com

L. 网络请求
来源：http://gwp.shuidangran.top

================================================================================
来源：http://frm.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://mqc.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://udj.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pgu.jyoumei.cn

JS:   await fetch(url)
来源：http://wqm.zhiwuduotai.top

TS:   await fetch(url)
来源：http://iht.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lwt.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://pjw.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ujy.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://snb.uphjek.com

[L02] 发送 POST JSON
来源：http://clx.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://hej.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mmo.vehdjk.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tzd.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cqk.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cis.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://geg.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://adb.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gga.zycfv.cn

[L03] 设置自定义请求头
来源：http://erc.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ezf.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ffb.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lww.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uwb.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cju.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yvc.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vbv.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dhw.nanxinkj.top

[L04] 设置超时
来源：http://jim.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://def.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uav.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vil.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qyd.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://epm.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mwi.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cev.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hfq.yongpay.top

[L05] 上传文件（multipart）
来源：http://oau.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://msr.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dvb.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gjr.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jpa.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wqa.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pzc.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dqn.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qyd.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://tyn.daxiang520.top

Py:   resp.json()
来源：http://oal.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://hik.jinghuilouyu.cn

JS:   await resp.json()
来源：http://vhb.xuanzx.com

TS:   await resp.json()
来源：http://upk.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vvf.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rtc.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://mlj.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rnj.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://ghb.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eys.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nvw.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://adp.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://ooc.tanke756.top

Java: resp.statusCode()
来源：http://kef.cheryme.top

Go:   resp.StatusCode
来源：http://nge.shzxlz.cn

Ruby: resp.code.to_i
来源：http://hvh.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://eyx.jqgufenzy.top

[L08] 并发请求多个地址
来源：http://wun.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://soj.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://gpk.jqgfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iqf.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uto.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ufh.cdnleiting.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yeh.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yck.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dum.hongshengwenyu.top

================================================================================
来源：http://orv.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://nuc.yuxming.cn


<!-- 参考信息 -->