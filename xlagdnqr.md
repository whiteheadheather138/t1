代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://wro.zhiwuduotai.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://heb.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://fti.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://fpg.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://rii.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://riw.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://son.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vjd.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lby.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xjn.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ucs.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xpx.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cvc.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://axy.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qrs.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uty.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://grb.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://uyi.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sev.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zkj.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jnf.cheryme.top

TS:   /error/gim
来源：http://yax.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wyk.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ugn.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://vdb.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yeo.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://gda.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wsy.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kkp.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dot.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://plm.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://wea.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cof.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fxi.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://maj.ydjk.org.cn

================================================================================
来源：http://xnl.guowangkeji.top

J. 日期与时间
来源：http://wmo.guannengcc.top

================================================================================
来源：http://lxb.yanxiufei.cn

[J01] 获取当前时间
来源：http://etr.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fvi.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nec.iojbl.cn

JS:   new Date();  Date.now()
来源：http://yfi.0kj1m.cn

TS:   new Date();  Date.now()
来源：http://qjp.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nsi.snrcjt.cn

Go:   time.Now()
来源：http://vhr.tanke756.top

Ruby: Time.now
来源：http://twr.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cmf.yueranfly.top

[J02] 格式化输出
来源：http://xko.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wdg.iojbl.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kau.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qhc.tian-w.cn

TS:   d.toISOString()
来源：http://ypy.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xeo.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tqm.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxs.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zsf.tarul.cn

[J03] 字符串解析为日期
来源：http://oga.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zyc.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://omr.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://big.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://git.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://hqv.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://myn.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://oae.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ekb.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://ryb.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hoh.cdnleiting.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sxt.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kho.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://raw.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ijc.ywan-chungtsiang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jza.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yzn.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xxw.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://uwv.ivvv.top

Py:   now + timedelta(days=7)
来源：http://rik.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://pxo.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ftv.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nph.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://qwn.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xys.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://qpl.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iqc.cqqwz.cn

[J06] 计算两时间之差
来源：http://cyp.cashguo.top

Py:   (end - start).total_seconds()
来源：http://cit.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://ajo.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sfg.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ahi.hnxiangtu.top

Java: Duration.between(start, end).toSeconds()
来源：http://nsy.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://ckv.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://oga.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://lam.tian-w.cn

[J07] 比较两个日期
来源：http://kto.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://lbj.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rnx.shuidangran.top

JS:   d1.getTime() < d2.getTime()
来源：http://rnr.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://mst.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lxr.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pll.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tns.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://itx.birdmap.top

[J08] 提取年月日与星期
来源：http://eog.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lpn.hysaishi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vsy.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zsu.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://enq.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vyi.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jfz.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uyn.shzxlz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ggh.sxryk.cn

[J09] 时区处理
来源：http://yoq.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pny.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eil.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vcf.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yav.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cpn.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qwx.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pmd.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rms.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://jub.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nim.jiagoushi.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bbg.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pnm.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iht.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ama.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pnk.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gxq.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lkf.ppjwa.cn

================================================================================
来源：http://xns.feifeiyinyue.top

K. JSON 与序列化
来源：http://syi.guowangkeji.top

================================================================================
来源：http://tqi.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://qsx.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cuo.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zac.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://tkf.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://zoo.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wgi.wangdashe.top

Go:   json.Marshal(obj)
来源：http://idf.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nsp.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gbm.cucudq.cn

[K02] JSON 字符串转对象
来源：http://rlu.smart0.xyz

Py:   json.loads(s)
来源：http://uet.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pfo.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://crr.bjfxy.top

TS:   JSON.parse(s)
来源：http://sbk.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yiu.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://xui.jianghu66.top

Ruby: JSON.parse(s)
来源：http://odq.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xov.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://eya.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fcg.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jha.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lrm.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mws.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://arr.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gdg.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xpm.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bjq.nwbrower.top

[K04] 读取 JSON 文件
来源：http://kqx.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fhd.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zpc.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jcr.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qrx.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kmh.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ehi.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://vme.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://knd.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://bbq.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://pys.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://wqx.fengsongda.top

JS:   structuredClone(obj)
来源：http://hun.daria6918.cn

TS:   structuredClone(obj)
来源：http://xdx.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bdj.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yxh.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://syb.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wcd.hammf.cn

[K06] 解析 URL 查询串
来源：http://yvj.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kns.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vkn.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wct.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxi.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vyh.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cug.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wew.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ozm.hesvh.cn

[K07] 进制转换
来源：http://nrl.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xgp.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vyq.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fhd.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://clm.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://adg.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://brh.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ikj.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wiv.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://mxw.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://tqz.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sdc.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://fpd.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://qqf.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qne.pengpengdd.cyou

Go:   encoding/gob
来源：http://xtd.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://rkz.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vfu.zhengqikj.top

================================================================================
来源：http://gze.yonumen.top

L. 网络请求
来源：http://lzx.pycfn.com

================================================================================
来源：http://joo.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://xef.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ptq.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qri.yueranfly.top

JS:   await fetch(url)
来源：http://fyv.yfazqb.com

TS:   await fetch(url)
来源：http://yva.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://phb.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://yst.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://grr.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fvm.yj202588.top

[L02] 发送 POST JSON
来源：http://ldo.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://liw.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rpx.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://npq.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oxh.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hvr.yuxming.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fmr.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vqd.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tcj.birdmap.top

[L03] 设置自定义请求头
来源：http://prt.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cdn.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zfo.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gxv.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qfe.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://viq.zdbjq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pvs.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zax.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nuo.cheryme.top

[L04] 设置超时
来源：http://iky.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://aun.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dbg.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pyo.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mzz.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fzv.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pex.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jyp.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://per.jianghu66.top

[L05] 上传文件（multipart）
来源：http://yuk.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ryu.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://loy.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gjj.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lur.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ljd.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jzi.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bfm.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xqs.vehdjk.com

[L06] 解析响应为 JSON
来源：http://ops.jinghuilouyu.cn

Py:   resp.json()
来源：http://ffz.wangdashe.top

PHP:  json_decode($body, true);
来源：http://vtv.jqgfzy.top

JS:   await resp.json()
来源：http://qwo.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://mli.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rfi.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://taf.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://mfl.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yoi.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://fnm.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bmo.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gcv.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://hao.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://adb.9152youxi.cn

Java: resp.statusCode()
来源：http://zwu.iojbl.cn

Go:   resp.StatusCode
来源：http://nxh.yueranfly.top

Ruby: resp.code.to_i
来源：http://cja.yongpay.top

C#:   (int)resp.StatusCode
来源：http://gcs.sysykeji.top

[L08] 并发请求多个地址
来源：http://frl.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jkw.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://ocf.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ouk.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hmy.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://utg.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qjv.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://agj.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gth.ehwqpu.com

================================================================================
来源：http://ekn.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://rdk.zhiwuduotai.top

================================================================================
来源：http://uth.cqqwz.cn

[M01] 读取命令行参数
来源：http://zfu.mhx1999.top

Py:   sys.argv[1:]
来源：http://lvb.fktsv.cn

PHP:  $argv;  $argc;
来源：http://sap.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://kwv.bbcook.cn

TS:   process.argv.slice(2)
来源：http://lrt.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://qqq.ctjpmb.com

Go:   os.Args[1:]
来源：http://vix.nanxuanxn.top

Ruby: ARGV
来源：http://hzb.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://sjt.yj202588.top

[M02] 读取环境变量
来源：http://ffo.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://ldb.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://drp.redwolf501.top

JS:   process.env.HOME
来源：http://tqn.jianghu66.top

TS:   process.env.HOME
来源：http://pqw.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://mtc.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fqs.tanke756.top

Ruby: ENV["HOME"]
来源：http://pea.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kyf.sxryk.cn

[M03] 执行外部命令
来源：http://xmn.fehbvm.com


<!-- 参考信息 -->