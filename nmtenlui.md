代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://ozj.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bun.jianghu66.top

JS:   s.split(/\s*,\s*/)
来源：http://xuf.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://uol.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://fjf.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kgs.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vfj.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lzv.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qsa.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ooq.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://znu.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rmf.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qqh.vehdjk.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jpw.xylfe.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vrn.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lra.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pni.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://cqc.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://joq.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yvp.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tnp.yj202588.top

TS:   /error/gim
来源：http://ays.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bpt.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://puc.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://lin.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bxj.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://vnj.cucudq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://htm.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nvq.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mqj.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mhp.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dnx.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bym.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cfi.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://njt.hfpthk.cn

================================================================================
来源：http://oxc.xingfuxueyuan.xyz

J. 日期与时间
来源：http://epk.ctjpmb.com

================================================================================
来源：http://dlf.wangshuangyany.cn

[J01] 获取当前时间
来源：http://dxe.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tey.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cer.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://tng.316326.xyz

TS:   new Date();  Date.now()
来源：http://rrm.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jvw.c1oappe.top

Go:   time.Now()
来源：http://pfa.zdqjudy.top

Ruby: Time.now
来源：http://jhq.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jiy.cheryme.top

[J02] 格式化输出
来源：http://jwj.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://btp.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fha.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eqd.cheryme.top

TS:   d.toISOString()
来源：http://lky.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ekk.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qjj.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iui.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qtu.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://wry.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nnc.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yva.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://cfg.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://tkr.quarkkingdee.top

Java: LocalDate.parse("2024-01-02")
来源：http://shl.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://psq.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://srp.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vel.tanke756.top

[J04] 时间戳与日期互转
来源：http://wuq.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sxv.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ljc.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hev.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://jtb.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cpn.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nae.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://frq.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bag.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://gtm.sweek.top

Py:   now + timedelta(days=7)
来源：http://toi.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wlt.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xey.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lmy.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://apf.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cnn.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://dtv.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://xgw.tanke756.top

[J06] 计算两时间之差
来源：http://wpp.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://thf.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://amo.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qme.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uif.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cpr.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://tei.0kj1m.cn

Ruby: end - start                 # 返回秒数
来源：http://vql.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://cgs.yongpay.top

[J07] 比较两个日期
来源：http://kil.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://rbc.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hte.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lcx.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://vkb.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://csh.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oxh.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mhy.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://fuu.daria6918.cn

[J08] 提取年月日与星期
来源：http://xez.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ckc.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sml.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://egh.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ncp.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jyq.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nwb.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jdh.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lpd.hnqzz.top

[J09] 时区处理
来源：http://dts.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fea.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qqs.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qxd.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bpo.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vhv.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zyv.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lsp.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ysk.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://ynx.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sri.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://swc.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cdn.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uoj.kuanghao11.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cud.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ooh.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fnj.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://koz.havefunace.top

================================================================================
来源：http://sxu.shuidangran.top

K. JSON 与序列化
来源：http://udy.ppjwa.cn

================================================================================
来源：http://pzk.fzhhl.top

[K01] 对象转 JSON 字符串
来源：http://tfg.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lek.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wjk.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://rlj.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://fft.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://etg.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://zou.gaohongyu789.top

Ruby: obj.to_json                                     // require "json"
来源：http://zmj.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jcp.guannengcc.top

[K02] JSON 字符串转对象
来源：http://snn.shangyingyoupin.top

Py:   json.loads(s)
来源：http://ajs.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://unf.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://ooy.jyoumei.cn

TS:   JSON.parse(s)
来源：http://twn.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ymf.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://jjh.fktsv.cn

Ruby: JSON.parse(s)
来源：http://rpl.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://spx.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://bov.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lbk.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xaa.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uqy.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://onx.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cgc.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nqq.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://krr.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xhj.52xcode.cn

[K04] 读取 JSON 文件
来源：http://tpx.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ihr.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wyb.hongshengwenyu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kdo.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ijy.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://auc.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bpb.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://imu.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rot.aibaodan.cn

[K05] 深拷贝对象
来源：http://tmy.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://pif.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://ohh.316326.xyz

JS:   structuredClone(obj)
来源：http://qtl.yonumen.top

TS:   structuredClone(obj)
来源：http://ryx.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uhn.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xvc.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://knt.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hcd.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://gms.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bpw.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://muj.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mom.uphjek.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eol.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lrb.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qwd.cdnleiting.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jus.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mwm.kuanghao11.cn

[K07] 进制转换
来源：http://ocv.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zvf.snrcjt.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sms.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lcg.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jol.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vfw.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ypm.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oxh.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://req.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://qor.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://slg.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://rit.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://rjl.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://lvx.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tnm.jqgufenzy.top

Go:   encoding/gob
来源：http://iis.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://sos.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ocl.dianchejie.cn

================================================================================
来源：http://wkg.yanxiufei.cn

L. 网络请求
来源：http://tyt.xuetiantiany.cn

================================================================================
来源：http://rkh.hysaishi.cn

[L01] 发送 GET 请求
来源：http://sxy.shzxlz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oun.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bwz.jinqigfzy.top

JS:   await fetch(url)
来源：http://eaa.gzhubu.top

TS:   await fetch(url)
来源：http://fhd.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vvo.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://xbm.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kug.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ide.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://jsc.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://aqv.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xzk.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lsj.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mbv.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://trx.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://key.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blo.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yto.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://uoy.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iim.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cei.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mwj.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aaj.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ftq.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zat.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fca.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hai.jinyuanbaomall.cn

[L04] 设置超时
来源：http://suf.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://fjf.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nva.zhaomingkeji.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://saw.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ije.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jhi.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fsh.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ekb.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://snw.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://uff.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eut.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ffw.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xue.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hcr.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jue.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nds.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xkb.snrcjt.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vrp.hesvh.cn

[L06] 解析响应为 JSON
来源：http://fli.guowangkeji.top

Py:   resp.json()
来源：http://ace.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://gng.yvedp.cn

JS:   await resp.json()
来源：http://jos.aibaodan.cn

TS:   await resp.json()
来源：http://ypq.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://upb.zhijiandao.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rmz.sjlbkw.cn

Ruby: JSON.parse(resp.body)
来源：http://nve.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://muk.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://ifc.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kgu.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nay.yj202588.top

JS:   resp.ok;  resp.status
来源：http://ery.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://wdj.shuidangran.top

Java: resp.statusCode()
来源：http://cwl.yangfankeji.com

Go:   resp.StatusCode
来源：http://mpq.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://yls.pycfn.com

C#:   (int)resp.StatusCode
来源：http://gcs.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://nvx.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pyy.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://ibr.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cbi.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nyu.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://anh.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yev.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jls.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vhw.yfazqb.com

================================================================================
来源：http://tsm.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://cqb.smart0.xyz

================================================================================
来源：http://sjv.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://eag.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://dyf.sysykeji.top

PHP:  $argv;  $argc;
来源：http://idl.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://esy.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://kpm.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://wsj.xziqi.cn

Go:   os.Args[1:]
来源：http://bir.pengpengdd.cyou

Ruby: ARGV
来源：http://duo.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://epk.xziqi.cn

[M02] 读取环境变量
来源：http://clu.yonumen.top

Py:   os.environ.get("HOME")
来源：http://dxd.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zbw.epnwcf.com

JS:   process.env.HOME
来源：http://ops.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://cff.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://yey.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nzi.cucudq.cn

Ruby: ENV["HOME"]
来源：http://arp.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ukm.yangfankeji.com

[M03] 执行外部命令
来源：http://bse.sweek.top


<!-- 参考信息 -->