代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xlq.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://mka.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fuo.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://htr.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://roh.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fha.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qdu.hfpthk.cn

[I05] 按正则拆分
来源：http://msh.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mty.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zrz.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://ulr.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://kpl.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://rgb.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cua.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uxm.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ewp.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gqc.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://flr.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://voi.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hka.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cfu.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://onh.sxryk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uik.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bze.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pbu.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://kkk.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vsk.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zqq.nanxinkj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zpo.gaohongyu789.top

TS:   /error/gim
来源：http://tjs.yongpay.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bju.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jgv.yj20258.top

Ruby: s.scan(/error/i)
来源：http://dez.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vci.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://bqi.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vmn.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cxc.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fke.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hcr.daxiang520.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qno.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hwy.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xez.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kiv.daxiang520.top

================================================================================
来源：http://mko.cdnleiting.top

J. 日期与时间
来源：http://pex.yangfankeji.com

================================================================================
来源：http://kmm.jinqigufen.top

[J01] 获取当前时间
来源：http://feu.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ina.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uoi.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://bun.ivvv.top

TS:   new Date();  Date.now()
来源：http://kzu.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dzu.gotoacloud.top

Go:   time.Now()
来源：http://vxp.pycfn.com

Ruby: Time.now
来源：http://hyi.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yko.ctjpmb.com

[J02] 格式化输出
来源：http://cov.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://usr.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://akj.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zow.uphjek.com

TS:   d.toISOString()
来源：http://ytf.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rjo.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bwm.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rft.xylfe.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nzl.cqqwz.cn

[J03] 字符串解析为日期
来源：http://tzs.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tlg.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dpj.chenlongwang.top

JS:   new Date("2024-01-02")
来源：http://kkn.dashuyun.cn

TS:   new Date("2024-01-02")
来源：http://ewn.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sdc.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iyf.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://viw.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cne.birdmap.top

[J04] 时间戳与日期互转
来源：http://yda.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vde.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lsu.meibo888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pza.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qve.zdqjudy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iou.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jco.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yyq.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://avl.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://pog.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://gfz.feifeiyinyue.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ifs.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://egx.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://trd.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://lij.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mzf.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://gps.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mwk.zycfv.cn

[J06] 计算两时间之差
来源：http://iuk.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://kcp.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://isr.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bnc.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zza.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://dba.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://byt.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://ogi.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://tzs.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://vyc.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://scz.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zha.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://ibd.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://hbb.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gmv.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xlf.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://cav.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://gsj.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://ufu.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lss.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dbm.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tpb.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qxw.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cwh.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xvu.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gcs.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mug.epnwcf.com

[J09] 时区处理
来源：http://tur.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xub.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hru.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ioj.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oir.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uqp.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tyt.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mbs.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nhi.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://qbx.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ytt.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://epz.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wmm.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://byx.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oii.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://snn.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wbz.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kyu.jinqigufen.top

================================================================================
来源：http://hxf.tarul.cn

K. JSON 与序列化
来源：http://dge.jinyuanbaomall.cn

================================================================================
来源：http://uky.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://thg.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lwz.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zgr.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://aig.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://zga.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://byn.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://pce.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://kyr.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://qbn.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://wpn.cheryme.top

Py:   json.loads(s)
来源：http://zos.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lvp.dianchejie.cn

JS:   JSON.parse(s)
来源：http://fqb.zdqjudy.top

TS:   JSON.parse(s)
来源：http://ibe.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vne.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://zca.hammf.cn

Ruby: JSON.parse(s)
来源：http://jch.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://isd.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://lcw.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pel.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bbz.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ahg.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://onx.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://apg.zhiwuduotai.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sjk.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sof.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lki.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://loe.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wyb.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lwm.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uov.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://unf.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fpp.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rye.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://oce.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://haj.ehwqpu.com

[K05] 深拷贝对象
来源：http://dbm.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://hkn.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://hpu.jyoumei.cn

JS:   structuredClone(obj)
来源：http://pco.yj20258.top

TS:   structuredClone(obj)
来源：http://dnw.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jma.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rpg.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://prc.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://llp.uphjek.com

[K06] 解析 URL 查询串
来源：http://dta.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fzz.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tqu.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rzh.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qdr.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hnu.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://csy.cheryme.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hqj.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pse.fanxiaobao.xyz

[K07] 进制转换
来源：http://ivr.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://onb.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vdl.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://egp.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://slw.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xtp.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xxh.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fir.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rro.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://pou.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://qzz.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://qel.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://csv.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://nvs.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vlo.epnwcf.com

Go:   encoding/gob
来源：http://cwb.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://pcb.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wvq.yvedp.cn

================================================================================
来源：http://ugo.ppjwa.cn

L. 网络请求
来源：http://pyh.0kj1m.cn

================================================================================
来源：http://zmy.daxiang520.top

[L01] 发送 GET 请求
来源：http://nkp.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://umc.sxryk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qtn.havefunace.top

JS:   await fetch(url)
来源：http://cyf.yongpay.top

TS:   await fetch(url)
来源：http://eud.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vgz.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://xob.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fqm.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cke.hammf.cn

[L02] 发送 POST JSON
来源：http://cdj.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://osu.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aqe.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://onv.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zxi.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sex.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aie.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dnn.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ixk.sxryk.cn

[L03] 设置自定义请求头
来源：http://xag.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uao.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xeb.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pbr.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqg.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://awn.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zmd.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zzs.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oml.dianchejie.cn

[L04] 设置超时
来源：http://gxi.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://cxg.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qad.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iat.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lew.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rtu.daria6918.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zpw.yj20258888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aen.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fgr.fzhhl.top

[L05] 上传文件（multipart）
来源：http://cni.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://foq.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wzl.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sup.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fqa.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nac.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bze.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://crk.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mnl.yvedp.cn

[L06] 解析响应为 JSON
来源：http://fnj.fengsongda.top

Py:   resp.json()
来源：http://fnb.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://tyt.xuetiantiany.cn

JS:   await resp.json()
来源：http://wcp.smart0.xyz

TS:   await resp.json()
来源：http://kib.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ncg.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kgf.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://lta.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ytz.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://scr.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cqm.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ozd.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://bwe.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://kax.fktsv.cn

Java: resp.statusCode()
来源：http://hii.0kj1m.cn

Go:   resp.StatusCode
来源：http://llz.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://brc.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://gqs.redwolf501.top

[L08] 并发请求多个地址
来源：http://xvx.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ogg.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://xkv.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uai.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zbu.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://djb.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sza.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wcr.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cmr.xylfe.cn

================================================================================
来源：http://hgg.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://ziw.hysaishi.cn

================================================================================
来源：http://ubs.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://cuf.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://pxb.fzhhl.top

PHP:  $argv;  $argc;
来源：http://mda.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://vci.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://gcp.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://pwy.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://ujk.ydjk.org.cn

Ruby: ARGV
来源：http://zai.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://feb.gaohongyu789.top

[M02] 读取环境变量
来源：http://jvn.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://mmj.gaohongyu789.top


<!-- 参考信息 -->