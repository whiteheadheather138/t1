代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://iyw.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xfl.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mfm.wangshuangyany.cn

[I05] 按正则拆分
来源：http://cio.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vgq.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://shm.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://qhp.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://zzg.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://sdo.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ifu.nanxuanxn.top

Ruby: s.split(/\s*,\s*/)
来源：http://dve.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hse.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://enr.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vpu.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fhh.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nbz.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eky.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wew.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bad.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rxf.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iwv.hcnkem.com

[I07] 忽略大小写与多行模式
来源：http://xmx.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ocb.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://suu.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qiy.jinyuanbaomall.cn

TS:   /error/gim
来源：http://tws.ctjpmb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fbi.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cjc.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://lwf.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tra.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://afk.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nsk.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zbk.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zru.hywenlv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xxi.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fmp.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oli.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jvz.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vfj.chenjidiqi.icu

================================================================================
来源：http://onp.shanyushiyangkeji.top

J. 日期与时间
来源：http://uza.dashuyun.cn

================================================================================
来源：http://qxc.jiagoushi.top

[J01] 获取当前时间
来源：http://ycm.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://szs.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hkt.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://khe.meibo888.top

TS:   new Date();  Date.now()
来源：http://vuj.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fep.xinyue.icu

Go:   time.Now()
来源：http://fzz.fanxiaobao.xyz

Ruby: Time.now
来源：http://rgh.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lrg.haohaochexian.top

[J02] 格式化输出
来源：http://hbc.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jzs.sxryk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wik.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nnx.cheryme.top

TS:   d.toISOString()
来源：http://rnw.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xzf.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fqc.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jyb.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vlv.hcnkem.com

[J03] 字符串解析为日期
来源：http://qax.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tjq.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ijk.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://rot.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://adx.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://ucf.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cpi.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://xrx.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lrr.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://cgo.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ses.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ato.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zwh.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ufk.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mth.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bet.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uyr.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://anj.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://aad.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://hvf.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://rez.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hok.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fdz.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://sdm.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://alj.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://pkt.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fbi.mhx1999.top

[J06] 计算两时间之差
来源：http://asz.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://znx.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://qkq.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jix.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ocn.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://idp.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://mpz.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://ecg.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://jqh.mhx1999.top

[J07] 比较两个日期
来源：http://nip.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://mdv.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mpy.cashguo.top

JS:   d1.getTime() < d2.getTime()
来源：http://wav.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bmu.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oal.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://epl.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://npg.shzxlz.cn

C#:   d1 < d2;  d1 == d2
来源：http://abn.fengsongda.top

[J08] 提取年月日与星期
来源：http://oai.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ufb.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lid.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pmo.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dzu.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hxr.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ufe.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ghu.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ybc.jqgufenzy.top

[J09] 时区处理
来源：http://klt.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lko.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jrx.cqqwz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mif.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jtk.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jms.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vmb.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xou.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jul.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://bps.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://uey.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yiq.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cnc.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pkj.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://emk.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://prp.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qaa.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zzy.gotoacloud.top

================================================================================
来源：http://noi.jinghuilouyu.cn

K. JSON 与序列化
来源：http://kid.iojbl.cn

================================================================================
来源：http://ycc.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://kto.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yup.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kab.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://tph.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://iyd.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://agt.vehdjk.com

Go:   json.Marshal(obj)
来源：http://xeb.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://nga.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qmh.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://dxr.yangfankeji.com

Py:   json.loads(s)
来源：http://hjz.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jpi.svipenyu.cn

JS:   JSON.parse(s)
来源：http://mps.yangfankeji.com

TS:   JSON.parse(s)
来源：http://npx.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://akf.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://can.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://rzz.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nfu.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://axf.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vsn.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ebc.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cgd.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ttx.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://arf.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://udz.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://oyx.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fdr.shuidangran.top

[K04] 读取 JSON 文件
来源：http://oba.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tmu.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mae.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kne.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xhn.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lzq.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zbk.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cjr.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fsg.yongpay.top

[K05] 深拷贝对象
来源：http://sez.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://elz.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://kbo.ivvv.top

JS:   structuredClone(obj)
来源：http://iwi.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://yod.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ufm.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xgm.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cdn.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://vys.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://cms.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bul.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nql.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nka.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aap.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zwy.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dzp.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nwx.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mrv.yfazqb.com

[K07] 进制转换
来源：http://oiy.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://usn.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yjh.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vwr.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ddf.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qhv.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sli.tianlin.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eav.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uvl.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://stj.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://icn.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://egj.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://ezj.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://jar.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iic.haohaochexian.top

Go:   encoding/gob
来源：http://gjq.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://qqd.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wjg.xziqi.cn

================================================================================
来源：http://tnm.fktsv.cn

L. 网络请求
来源：http://qwx.hesvh.cn

================================================================================
来源：http://fra.yongpay.top

[L01] 发送 GET 请求
来源：http://jph.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ybw.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ibq.aibaodan.cn

JS:   await fetch(url)
来源：http://ezc.hesvh.cn

TS:   await fetch(url)
来源：http://ekx.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lfs.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://ysv.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://osg.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fiz.52xcode.cn

[L02] 发送 POST JSON
来源：http://zul.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://omr.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dmr.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kau.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://awx.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ncq.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kjm.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dri.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wjf.ydzc1.top

[L03] 设置自定义请求头
来源：http://vdq.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rto.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aig.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yte.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gei.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uuc.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ruf.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hrz.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dil.yuanzhike.top

[L04] 设置超时
来源：http://wjf.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://gtp.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rvx.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://now.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qlc.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://coi.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fbf.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uwy.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iae.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://xoh.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zds.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pga.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nzy.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jkn.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uxm.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://heg.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pov.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://urp.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://nxn.feifeiyinyue.top

Py:   resp.json()
来源：http://jfi.pycfn.com

PHP:  json_decode($body, true);
来源：http://dlo.52xcode.cn

JS:   await resp.json()
来源：http://uif.ydzc1.top

TS:   await resp.json()
来源：http://sfd.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iat.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hzv.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://typ.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eof.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://yia.sjlbkw.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://etz.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://obk.hnxiangtu.top

JS:   resp.ok;  resp.status
来源：http://orm.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://kfl.kuanghao11.cn

Java: resp.statusCode()
来源：http://lht.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://ztd.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://ipq.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://ypa.bbcook.cn

[L08] 并发请求多个地址
来源：http://mep.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uvq.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://axx.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mjs.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zos.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zki.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nuf.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hxn.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xhn.chenlongwang.top

================================================================================
来源：http://ids.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://zxk.shanyushiyangkeji.top

================================================================================
来源：http://eni.svipenyu.cn

[M01] 读取命令行参数
来源：http://osq.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://cgq.yj20258888.top

PHP:  $argv;  $argc;
来源：http://rzv.cheryme.top

JS:   process.argv.slice(2)
来源：http://weh.jianghu66.top

TS:   process.argv.slice(2)
来源：http://eku.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://xkl.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://xyh.meibo888.top

Ruby: ARGV
来源：http://kzu.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://kvj.xylfe.cn

[M02] 读取环境变量
来源：http://vxi.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://spf.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pyf.0kj1m.cn

JS:   process.env.HOME
来源：http://gev.snrcjt.cn

TS:   process.env.HOME
来源：http://wxe.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://gdu.zycfv.cn


<!-- 参考信息 -->