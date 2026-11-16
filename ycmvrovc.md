代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://roz.hnxiangtu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://znj.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ogl.yueranfly.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bfd.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hrd.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yjt.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gqw.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zur.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vnu.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rtu.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tbm.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zrh.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aec.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://ykq.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vjj.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://itm.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xtn.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://mpz.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ljq.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gdw.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://pxo.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://woh.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://cxl.pengpengdd.cyou

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lal.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ady.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jxn.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iof.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ltu.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zle.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pdj.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ijq.pycfn.com

================================================================================
来源：http://qab.316326.xyz

J. 日期与时间
来源：http://vno.gotoacloud.top

================================================================================
来源：http://sxk.yongpay.top

[J01] 获取当前时间
来源：http://qxy.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://elg.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://utp.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://rye.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://zkc.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mjv.vqdsnc.cn

Go:   time.Now()
来源：http://wua.dianchejie.cn

Ruby: Time.now
来源：http://xjj.chenlongwang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://plc.svipenyu.cn

[J02] 格式化输出
来源：http://yfq.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://quy.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lym.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fzu.shangyingyoupin.top

TS:   d.toISOString()
来源：http://ecu.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ftr.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gls.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kkw.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eiw.sxryk.cn

[J03] 字符串解析为日期
来源：http://edk.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qpl.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xdc.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://pqc.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://rxn.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://deu.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sgn.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://fzj.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gqe.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://ako.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cjq.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kls.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rnz.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://sws.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uvd.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yrn.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://izn.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ywg.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://zeq.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://bsx.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://mby.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gwk.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jdu.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://ctx.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://voz.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://vqh.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://pcx.sxryk.cn

[J06] 计算两时间之差
来源：http://sfd.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://ega.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://ege.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xum.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rec.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jpg.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://wwg.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://obb.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://gjt.zhongyouzk.top

[J07] 比较两个日期
来源：http://hip.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://wly.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ccq.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zyi.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://lvn.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uwe.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wha.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://znx.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://mgy.cqqwz.cn

[J08] 提取年月日与星期
来源：http://wtt.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://njg.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ppl.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gut.aizwys.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pek.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yxw.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://doq.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lsz.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gxe.zhiwuduotai.top

[J09] 时区处理
来源：http://hag.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bbi.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://geq.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jtm.fanxiaobao.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sot.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ffo.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hcm.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jkb.ydjk.org.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yhy.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://did.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uwe.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fix.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xya.havefunace.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yoi.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ycr.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jog.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ulf.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hel.iojbl.cn

================================================================================
来源：http://jyw.c1oappe.top

K. JSON 与序列化
来源：http://psg.jlsjyb.cn

================================================================================
来源：http://xte.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://vdf.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hym.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lko.316326.xyz

JS:   JSON.stringify(obj)
来源：http://jfo.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://zng.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ujg.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://pbi.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://krw.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://rek.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://diq.redwolf501.top

Py:   json.loads(s)
来源：http://irk.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://psn.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://sti.zdqjudy.top

TS:   JSON.parse(s)
来源：http://zly.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mrp.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://czg.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://jhs.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cht.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://zvs.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ysl.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tqu.uphjek.com

JS:   JSON.stringify(obj, null, 2)
来源：http://sqt.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://byx.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jbz.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dpn.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://zdd.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hhd.havefunace.top

[K04] 读取 JSON 文件
来源：http://cry.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ori.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lch.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dfk.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dja.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xen.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lrg.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qfn.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oxy.hfpthk.cn

[K05] 深拷贝对象
来源：http://vcq.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://bob.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://jve.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://oex.redwolf501.top

TS:   structuredClone(obj)
来源：http://zvg.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yro.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yxg.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ygr.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oys.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://dte.pycfn.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://idd.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jfj.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ggi.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qvz.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ymc.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hdu.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pmq.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://afo.cucudq.cn

[K07] 进制转换
来源：http://skx.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pvy.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wbx.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nbc.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bmc.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aaj.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ziv.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qrr.cheryme.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ihk.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://jnb.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://osc.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xyw.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://pev.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://jxi.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hzr.ydzc1.top

Go:   encoding/gob
来源：http://ojn.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://xpc.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ris.9152youxi.cn

================================================================================
来源：http://oft.iojbl.cn

L. 网络请求
来源：http://wvh.hongshengwenyu.top

================================================================================
来源：http://tae.wangdashe.top

[L01] 发送 GET 请求
来源：http://osz.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bav.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kap.yuxming.cn

JS:   await fetch(url)
来源：http://ozb.quarkkingdee.top

TS:   await fetch(url)
来源：http://qid.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://szs.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://umd.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://xch.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uyh.andypj.xyz

[L02] 发送 POST JSON
来源：http://evk.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vxo.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fhx.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cbx.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lqp.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rmt.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lne.jianghu66.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ajw.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rdw.hammf.cn

[L03] 设置自定义请求头
来源：http://cpx.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dog.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fgf.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewk.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ovs.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jnh.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dza.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://elv.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://czg.ivvv.top

[L04] 设置超时
来源：http://okr.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://apk.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yfj.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://atq.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eap.quarkkingdee.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wch.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pds.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wjm.xziqi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dll.xylfe.cn

[L05] 上传文件（multipart）
来源：http://gpv.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nvu.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wbc.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oaj.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tmf.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iqz.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cay.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aew.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mni.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://vpb.aibaodan.cn

Py:   resp.json()
来源：http://iqm.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://xvx.mhx1999.top

JS:   await resp.json()
来源：http://epx.xuanzx.com

TS:   await resp.json()
来源：http://yyb.aizwys.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ntp.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yjm.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://uvm.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ril.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://scc.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kir.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fdx.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://kxd.bjfxy.top

TS:   resp.ok;  resp.status
来源：http://wrm.ctjpmb.com

Java: resp.statusCode()
来源：http://una.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://zpg.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://foh.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://rrf.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://lgq.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rbq.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://oyj.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cyf.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tjj.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hwk.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://twk.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yfl.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mcg.nwbrower.top

================================================================================
来源：http://wcz.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://mob.chenlongwang.top

================================================================================
来源：http://zox.9152youxi.cn

[M01] 读取命令行参数
来源：http://zxg.snrcjt.cn

Py:   sys.argv[1:]
来源：http://npw.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://hdp.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://llh.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://pkg.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://iaq.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://uqr.daxiang520.top

Ruby: ARGV
来源：http://ksu.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://qzj.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://rzd.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://opp.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ryg.dianchejie.cn

JS:   process.env.HOME
来源：http://slt.zhixingplan.top

TS:   process.env.HOME
来源：http://wkw.xziqi.cn

Java: System.getenv("HOME")
来源：http://zgu.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xhj.tanke756.top

Ruby: ENV["HOME"]
来源：http://nsc.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zbc.guannengcc.top

[M03] 执行外部命令
来源：http://lvh.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kaz.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vxn.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://usc.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bpy.vqdsnc.cn


<!-- 参考信息 -->