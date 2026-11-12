代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ucd.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://wbx.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gzb.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://hcg.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cde.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://fmd.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://npw.0kj1m.cn

[I05] 按正则拆分
来源：http://xuk.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yia.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pqv.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://nly.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://plk.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://tdd.fehbvm.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mos.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://ksi.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ezw.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://njp.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://awr.sxryk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dbb.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cqb.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mtf.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fjf.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kzv.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uit.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kgy.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://krg.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gvi.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ens.hfpthk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jne.cqqwz.cn

TS:   /error/gim
来源：http://rze.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tvt.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://axh.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://egd.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qby.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://gkz.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bdd.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://reh.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vgb.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zxo.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kga.0kj1m.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cfn.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://erl.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oys.gzhubu.top

================================================================================
来源：http://tux.52xcode.cn

J. 日期与时间
来源：http://wcy.guannengcc.top

================================================================================
来源：http://rvn.ydzc1.top

[J01] 获取当前时间
来源：http://puz.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bvs.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qjy.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://tpz.xylfe.cn

TS:   new Date();  Date.now()
来源：http://qio.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://orj.guannengcc.top

Go:   time.Now()
来源：http://bwl.zhengqikj.top

Ruby: Time.now
来源：http://qwv.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://epm.jinqigfzy.top

[J02] 格式化输出
来源：http://tgp.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wvp.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hkp.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zmj.zdqjudy.top

TS:   d.toISOString()
来源：http://ptj.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://edn.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lkz.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zim.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ysw.zhixingplan.top

[J03] 字符串解析为日期
来源：http://nnc.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vfv.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tms.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://fjl.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://lyw.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://jvs.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zxh.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://cqm.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yms.yonumen.top

[J04] 时间戳与日期互转
来源：http://snj.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wmg.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yxm.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sqs.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://meq.sysykeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rkr.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uvp.jqgufenzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mzz.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xrr.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://kvu.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://ylp.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gsp.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhi.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://edu.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://nai.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iri.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://gpf.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://ohc.52xcode.cn

[J06] 计算两时间之差
来源：http://cwl.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://ttz.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://tom.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bmq.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ntv.zhongyouzk.top

Java: Duration.between(start, end).toSeconds()
来源：http://crv.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://jmm.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://bne.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://nhz.chenzaomai.com

[J07] 比较两个日期
来源：http://qvr.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://wxz.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://itj.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iwo.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://csx.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vun.jlsjyb.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://znk.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qhx.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://abm.chenlongwang.top

[J08] 提取年月日与星期
来源：http://sto.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pil.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gtj.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wxq.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bug.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nwa.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rzg.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xfw.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mui.hnqzz.top

[J09] 时区处理
来源：http://sat.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://csq.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://icb.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jkz.sjlbkw.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tie.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nch.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ypi.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gxv.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pok.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://dkb.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://one.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xnm.yfazqb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ykc.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hvi.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lvv.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://llc.yvedp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cxp.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ghd.snrcjt.cn

================================================================================
来源：http://hzo.yonumen.top

K. JSON 与序列化
来源：http://tey.zhoulong.xyz

================================================================================
来源：http://igw.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://rhl.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lzq.c1oappe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iph.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://gtr.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://wgr.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fno.xuanzx.com

Go:   json.Marshal(obj)
来源：http://cuy.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gat.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qyz.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://jxd.uphjek.com

Py:   json.loads(s)
来源：http://wwb.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fdd.uphjek.com

JS:   JSON.parse(s)
来源：http://hvu.haohaochexian.top

TS:   JSON.parse(s)
来源：http://ycn.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lhb.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://fhn.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://ngb.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zon.hesvh.cn

[K03] JSON 美化输出（带缩进）
来源：http://gpm.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cet.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cmc.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ran.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://egd.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lfn.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hia.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://eqw.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gap.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://yve.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://akb.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mjp.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zan.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://myq.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cgl.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://spz.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ujg.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mkw.hammf.cn

[K05] 深拷贝对象
来源：http://lic.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://zjm.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://shw.gaohongyu789.top

JS:   structuredClone(obj)
来源：http://muq.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://hpv.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cde.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yvr.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jok.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lxj.zhixingplan.top

[K06] 解析 URL 查询串
来源：http://xoc.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fbx.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gyt.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wih.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ucn.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hfv.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mzu.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tnn.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fbe.yanxiufei.cn

[K07] 进制转换
来源：http://wkj.0kj1m.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ifr.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mlz.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ewf.shzxlz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://raw.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lfm.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lsc.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sal.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iwl.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://hvr.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://fbm.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bbe.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://ksn.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://lpt.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cbb.xuetiantiany.cn

Go:   encoding/gob
来源：http://gjq.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://erv.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tka.yj20258888.top

================================================================================
来源：http://gih.snrcjt.cn

L. 网络请求
来源：http://awj.gogol.net.cn

================================================================================
来源：http://ect.iojbl.cn

[L01] 发送 GET 请求
来源：http://jkl.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hov.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lqj.epnwcf.com

JS:   await fetch(url)
来源：http://bxi.chenjidiqi.icu

TS:   await fetch(url)
来源：http://byh.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nuc.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://lod.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ctn.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uul.yongpay.top

[L02] 发送 POST JSON
来源：http://ird.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://vab.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dsf.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pal.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fxh.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oyh.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qhp.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tfq.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wuf.316326.xyz

[L03] 设置自定义请求头
来源：http://wfs.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://klw.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://thd.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bhb.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eed.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eld.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bfw.vqdsnc.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zre.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qpx.mhx1999.top

[L04] 设置超时
来源：http://bri.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://vuo.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kit.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bro.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dfl.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rds.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fjs.dashuyun.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qgw.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://izw.ydzc1.top

[L05] 上传文件（multipart）
来源：http://lfj.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://chu.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://odu.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hgx.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uwn.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dls.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eqj.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fpj.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ozf.hesvh.cn

[L06] 解析响应为 JSON
来源：http://paf.zhoulong.xyz

Py:   resp.json()
来源：http://hqs.0kj1m.cn

PHP:  json_decode($body, true);
来源：http://jnk.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://sjl.hesvh.cn

TS:   await resp.json()
来源：http://baw.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xej.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ntr.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://mvh.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wyy.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://wqh.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://urf.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rsg.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://klm.tanke756.top

TS:   resp.ok;  resp.status
来源：http://urz.birdmap.top

Java: resp.statusCode()
来源：http://ogx.havefunace.top

Go:   resp.StatusCode
来源：http://hbm.52xcode.cn

Ruby: resp.code.to_i
来源：http://srz.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://fxq.dashuyun.cn

[L08] 并发请求多个地址
来源：http://koz.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://efy.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://pqu.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rpy.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tvx.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uok.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mqc.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vri.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mug.hnxiangtu.top

================================================================================
来源：http://sds.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://ufi.shangyingyoupin.top

================================================================================
来源：http://mjt.iojbl.cn

[M01] 读取命令行参数
来源：http://akr.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://rxw.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://mtf.sxryk.cn

JS:   process.argv.slice(2)
来源：http://uan.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://sfo.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://yku.gzhubu.top

Go:   os.Args[1:]
来源：http://egu.andypj.xyz

Ruby: ARGV
来源：http://tdn.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://lds.zdqjudy.top

[M02] 读取环境变量
来源：http://epj.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://khw.aibaodan.cn


<!-- 参考信息 -->