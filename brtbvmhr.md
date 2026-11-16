代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://bvj.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gbe.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hsy.sjlbkw.cn

[I05] 按正则拆分
来源：http://ngt.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wso.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://siy.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://nxs.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://ndc.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://lwe.yfazqb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jva.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://lpw.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dmm.xingfuxueyuan.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ppd.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://slw.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jgj.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jyu.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qjf.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zdf.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sak.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jyv.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wrh.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://rlk.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yto.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ftz.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jib.hysaishi.cn

TS:   /error/gim
来源：http://ltl.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dfz.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kmq.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://pif.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ozt.mhx1999.top

[I08] 贪婪与非贪婪匹配
来源：http://gda.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jfx.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vet.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ywu.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://suj.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ugl.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sdx.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vuz.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xyd.yongpay.top

================================================================================
来源：http://jrq.zdbjq.cn

J. 日期与时间
来源：http://moq.uphjek.com

================================================================================
来源：http://rwu.yongpay.top

[J01] 获取当前时间
来源：http://meb.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ycp.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://czb.fktsv.cn

JS:   new Date();  Date.now()
来源：http://moe.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://fum.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://erz.sweek.top

Go:   time.Now()
来源：http://stv.zhaomingkeji.xyz

Ruby: Time.now
来源：http://hhq.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tpf.fktsv.cn

[J02] 格式化输出
来源：http://xcn.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bce.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vaw.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zzd.hysaishi.cn

TS:   d.toISOString()
来源：http://qza.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://phw.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ylq.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ckj.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nmo.zhengqikj.top

[J03] 字符串解析为日期
来源：http://cin.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lap.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tsn.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://jks.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://sgu.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hkq.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nvb.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://kcf.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yve.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://flr.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jmc.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fno.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pao.ydzc1.top

TS:   Math.floor(Date.now() / 1000)
来源：http://udt.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jah.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://clj.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eiv.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zzx.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://ypc.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://cni.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://imh.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oxx.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gqj.ybcxt.top

Java: LocalDate.now().plusDays(7)
来源：http://soh.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://irq.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://tpo.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gbd.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://mru.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://byp.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://joc.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ons.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lja.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://zxh.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://ndr.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://max.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://eix.cucudq.cn

[J07] 比较两个日期
来源：http://xvx.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://gxh.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lwd.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://wza.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://syc.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vhb.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cuk.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://xmn.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://ugq.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://aiv.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kxw.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mjf.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qer.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pln.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://onl.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://geg.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://isr.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://acx.yangfankeji.com

[J09] 时区处理
来源：http://sog.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mmw.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lam.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qpy.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ziu.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lqj.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zif.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eyx.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://utk.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://aqs.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://zor.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wrc.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eta.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vwr.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ebi.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nuu.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jgs.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ldy.zdbjq.cn

================================================================================
来源：http://fsx.pengpengdd.cyou

K. JSON 与序列化
来源：http://qcr.316326.xyz

================================================================================
来源：http://stl.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://hng.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nhw.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://neq.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://xna.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://zdg.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kdc.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://xln.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://png.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://njp.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://bkb.bbcook.cn

Py:   json.loads(s)
来源：http://lvn.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://che.yvedp.cn

JS:   JSON.parse(s)
来源：http://dob.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://yza.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tss.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://ggv.sxryk.cn

Ruby: JSON.parse(s)
来源：http://kzy.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://igi.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://syu.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fah.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wfw.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kng.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qml.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cuu.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://het.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://jit.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ixn.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://ull.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://umo.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aez.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gwv.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jpc.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vxk.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xot.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sts.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hzw.cqqwz.cn

[K05] 深拷贝对象
来源：http://yia.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://reg.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://plu.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://jpn.wangdashe.top

TS:   structuredClone(obj)
来源：http://hpa.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xff.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zrb.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vpu.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bvg.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://efa.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qrg.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oxz.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mjs.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rgf.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pxr.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xen.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://asw.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://thj.ybcxt.top

[K07] 进制转换
来源：http://neq.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uyu.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lgx.shzxlz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://twi.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://miz.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://trt.vehdjk.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eyx.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lkw.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vrl.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://cgd.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://qeb.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nzm.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://qyt.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://xun.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hqq.ehwqpu.com

Go:   encoding/gob
来源：http://wvl.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://zgk.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cel.jqgfzy.top

================================================================================
来源：http://jma.xuetiantiany.cn

L. 网络请求
来源：http://dhg.fanxiaobao.xyz

================================================================================
来源：http://qbl.svipenyu.cn

[L01] 发送 GET 请求
来源：http://zzg.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xog.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ieb.yj20258.top

JS:   await fetch(url)
来源：http://ddr.tarul.cn

TS:   await fetch(url)
来源：http://afu.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qdy.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://wic.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wpq.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://grv.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://zrw.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lbx.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ctw.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fly.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tsr.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jei.andypj.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eui.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lcj.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ppd.aibaodan.cn

[L03] 设置自定义请求头
来源：http://fra.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://elo.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://njr.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wpm.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ciu.cashguo.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cdr.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uqn.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rjt.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ims.ivvv.top

[L04] 设置超时
来源：http://los.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://ifw.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rdl.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mvk.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aeh.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://avc.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://llb.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vxh.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tkp.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://toy.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pyb.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xmb.gogol.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vcx.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vhy.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ggp.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yft.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sxr.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vpl.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://kwz.tanke756.top

Py:   resp.json()
来源：http://akm.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://rbx.zhongyouzk.top

JS:   await resp.json()
来源：http://dzn.zhiwuduotai.top

TS:   await resp.json()
来源：http://sgi.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zlz.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fnq.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://yza.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qoa.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://dnh.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kul.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wmv.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://sag.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://zgd.jyoumei.cn

Java: resp.statusCode()
来源：http://fib.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://oul.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://lyj.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://vhp.jianghu66.top

[L08] 并发请求多个地址
来源：http://cgv.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tjn.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://wqr.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jte.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xkz.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iog.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bav.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://irv.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xou.yonumen.top

================================================================================
来源：http://daw.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://oxg.andypj.xyz

================================================================================
来源：http://kkk.tanke756.top

[M01] 读取命令行参数
来源：http://hic.iojbl.cn

Py:   sys.argv[1:]
来源：http://tqu.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://itd.tian-w.cn

JS:   process.argv.slice(2)
来源：http://fwz.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://odf.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://pcy.pycfn.com

Go:   os.Args[1:]
来源：http://quv.chenlongwang.top

Ruby: ARGV
来源：http://vir.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://deg.quarkkingdee.top

[M02] 读取环境变量
来源：http://lci.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://ovs.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bcl.bbcook.cn

JS:   process.env.HOME
来源：http://klh.snrcjt.cn

TS:   process.env.HOME
来源：http://rkv.316326.xyz

Java: System.getenv("HOME")
来源：http://auj.fehbvm.com


<!-- 参考信息 -->