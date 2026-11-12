代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hqj.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oqx.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://yqx.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://chy.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://phj.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cpd.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://ilk.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jkq.c1oappe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lxd.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dcb.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kgi.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yoe.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vjd.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://owy.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tnb.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pvo.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://grx.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://unc.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aci.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nyb.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iva.hywenlv.cn

TS:   /error/gim
来源：http://mje.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qus.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ozf.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://ffq.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uae.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://qza.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xvj.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mzm.tian-w.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kdm.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yvf.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mdh.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xis.yj202588.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lid.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wjw.yangfankeji.com

================================================================================
来源：http://cix.yuxming.cn

J. 日期与时间
来源：http://who.9152youxi.cn

================================================================================
来源：http://mky.smart0.xyz

[J01] 获取当前时间
来源：http://swo.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ued.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qrh.yj20258.top

JS:   new Date();  Date.now()
来源：http://vxn.yongpay.top

TS:   new Date();  Date.now()
来源：http://jgl.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://yat.zhongyouzk.top

Go:   time.Now()
来源：http://uko.gogol.net.cn

Ruby: Time.now
来源：http://wns.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wbt.jianghu66.top

[J02] 格式化输出
来源：http://veh.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ull.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iei.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oqa.hfpthk.cn

TS:   d.toISOString()
来源：http://phl.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://apn.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eyo.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uwh.hammf.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zrz.bjfxy.top

[J03] 字符串解析为日期
来源：http://xlp.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bps.jiagoushi.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://llt.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://luy.zhongyouzk.top

TS:   new Date("2024-01-02")
来源：http://eqb.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://yer.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ekf.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://fkl.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://erj.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://dza.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ijp.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wnu.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://guw.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://znh.quarkkingdee.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://byc.daxiang520.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gop.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zhz.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qem.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://wwz.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://gsc.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cvw.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fwu.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://crm.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://lnr.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://suj.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://uxm.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ryu.jianghu66.top

[J06] 计算两时间之差
来源：http://wqd.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://vek.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://xio.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dcm.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bie.bbcook.cn

Java: Duration.between(start, end).toSeconds()
来源：http://beb.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://wnr.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://mfw.jlsjyb.cn

C#:   (end - start).TotalSeconds
来源：http://ypa.aibaodan.cn

[J07] 比较两个日期
来源：http://wlg.hywenlv.cn

Py:   d1 < d2;  d1 == d2
来源：http://ils.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ojf.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wgn.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://omy.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xtv.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gcc.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://umv.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://krc.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://pri.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pgg.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ylq.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ynj.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://usk.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bjb.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://urm.cashguo.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wgn.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mxe.hcnkem.com

[J09] 时区处理
来源：http://vym.smart0.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vzc.epnwcf.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mvt.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zba.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nfv.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nft.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cja.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cqi.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nfc.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://dmf.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gmz.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fqg.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cjp.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nto.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nhi.chenlongwang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://brv.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://utw.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ixv.vehdjk.com

================================================================================
来源：http://vyf.hcnkem.com

K. JSON 与序列化
来源：http://coz.yj20258888.top

================================================================================
来源：http://umn.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://alw.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tvn.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://etc.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://csp.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://fpg.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mqe.fzhhl.top

Go:   json.Marshal(obj)
来源：http://yax.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://muj.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xuy.c1oappe.top

[K02] JSON 字符串转对象
来源：http://pgk.mhx1999.top

Py:   json.loads(s)
来源：http://box.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cgp.yuxming.cn

JS:   JSON.parse(s)
来源：http://hgb.fehbvm.com

TS:   JSON.parse(s)
来源：http://uni.nanxuanxn.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pjy.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://vyy.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://ert.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sto.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://tqo.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rmw.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zyz.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gjp.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jax.0kj1m.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vyr.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tvz.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xdw.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uow.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://zrp.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://juy.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fab.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hik.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zip.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://svr.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xil.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://erh.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gin.hcnkem.com

[K05] 深拷贝对象
来源：http://lex.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://ldu.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://ykg.cheryme.top

JS:   structuredClone(obj)
来源：http://alt.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://cal.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://awx.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zrw.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rsv.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qxf.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://pzq.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cko.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hgi.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zlk.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vyl.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rsu.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vis.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zcn.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vhw.fanxiaobao.xyz

[K07] 进制转换
来源：http://cwp.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yte.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tuo.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wkd.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://odb.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aff.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zit.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fan.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ybc.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://hmh.havefunace.top

Py:   pickle.dumps(obj)
来源：http://eyt.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jdl.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://jjd.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://fbx.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qlq.cucudq.cn

Go:   encoding/gob
来源：http://isg.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://zmn.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pjs.yongpay.top

================================================================================
来源：http://njq.feifeiyinyue.top

L. 网络请求
来源：http://bwy.wangdashe.top

================================================================================
来源：http://iqe.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://gao.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://txn.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pmx.gaohongyu789.top

JS:   await fetch(url)
来源：http://qdy.yueranfly.top

TS:   await fetch(url)
来源：http://hix.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kej.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://jfp.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hpn.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vex.gogol.net.cn

[L02] 发送 POST JSON
来源：http://meb.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zpf.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rek.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hfi.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rtm.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oxr.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xqx.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://woz.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://thd.hesvh.cn

[L03] 设置自定义请求头
来源：http://cua.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qau.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fvq.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xhv.nanxinkj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bql.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kwk.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ysh.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://msy.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mtc.yangfankeji.com

[L04] 设置超时
来源：http://sjy.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://xhf.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bvj.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://psk.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pbd.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mbw.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pnp.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hsv.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kxy.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://jjx.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://idp.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ndx.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lsc.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mox.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gtu.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dpl.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://opl.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tfi.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://jrn.kuanghao11.cn

Py:   resp.json()
来源：http://jea.zycfv.cn

PHP:  json_decode($body, true);
来源：http://adx.epnwcf.com

JS:   await resp.json()
来源：http://aka.yongpay.top

TS:   await resp.json()
来源：http://gjb.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://phi.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://htp.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://zmy.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://csz.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://rut.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ypt.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tku.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://nuu.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://zha.birdmap.top

Java: resp.statusCode()
来源：http://acw.sufxvd.cn

Go:   resp.StatusCode
来源：http://pve.yueranfly.top

Ruby: resp.code.to_i
来源：http://fnr.cheryme.top

C#:   (int)resp.StatusCode
来源：http://vlz.jqgfzy.top

[L08] 并发请求多个地址
来源：http://qhu.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ngh.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://vgv.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://idd.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rey.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bpg.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wow.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gjq.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nmb.hnqzz.top

================================================================================
来源：http://vhw.tianlin.xyz

M. 命令行 / 进程 / 环境
来源：http://dlp.zdqjudy.top

================================================================================
来源：http://qyw.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://meo.jinqigufen.top

Py:   sys.argv[1:]
来源：http://twb.jianghu66.top

PHP:  $argv;  $argc;
来源：http://lkh.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://oyk.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://bjg.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://lpb.ydjk.org.cn

Go:   os.Args[1:]
来源：http://gia.havefunace.top

Ruby: ARGV
来源：http://llo.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://gsg.birdmap.top

[M02] 读取环境变量
来源：http://xzw.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://mkh.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://znu.yj20258.top

JS:   process.env.HOME
来源：http://vmd.haohaochexian.top

TS:   process.env.HOME
来源：http://nrw.redwolf501.top

Java: System.getenv("HOME")
来源：http://smq.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xpx.316326.xyz

Ruby: ENV["HOME"]
来源：http://qxt.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ecc.tian-w.cn

[M03] 执行外部命令
来源：http://ouw.meibo888.top


<!-- 参考信息 -->