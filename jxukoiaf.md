代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://bln.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mnj.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vzf.bbcook.cn

[I05] 按正则拆分
来源：http://kct.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://cfx.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hvs.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://qua.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://mym.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://gtw.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uqj.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://cgb.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://piw.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rxe.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jcr.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tjg.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lii.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oho.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dhl.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://djw.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xxs.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://glw.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://hrx.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wsv.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sdb.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iov.uphjek.com

TS:   /error/gim
来源：http://wxh.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fcx.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pgr.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://kcr.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gwy.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://pzt.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oep.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zwr.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jlq.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://akc.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xws.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lcg.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zod.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jiu.yj20258.top

================================================================================
来源：http://req.jqgufenzy.top

J. 日期与时间
来源：http://fpi.nanxinkj.top

================================================================================
来源：http://cww.shzxlz.cn

[J01] 获取当前时间
来源：http://tsg.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://voa.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cez.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://mct.fengsongda.top

TS:   new Date();  Date.now()
来源：http://rhv.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ski.daxiang520.top

Go:   time.Now()
来源：http://kdh.sweek.top

Ruby: Time.now
来源：http://svr.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kuq.xylfe.cn

[J02] 格式化输出
来源：http://yfh.hesvh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jlo.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mza.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rms.zycfv.cn

TS:   d.toISOString()
来源：http://yvn.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oya.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cgo.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hsa.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ugr.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://vrp.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bcq.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xwk.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://ldx.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://wbg.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://bsz.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tte.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://kpc.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vla.meibo888.top

[J04] 时间戳与日期互转
来源：http://pzr.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zub.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://klc.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rtc.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://jfa.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ard.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rgx.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qbc.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jpz.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://vuj.yongpay.top

Py:   now + timedelta(days=7)
来源：http://scv.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qpt.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cer.xinyue.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wcp.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://lvn.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zif.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://sbu.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://lrt.cdnleiting.top

[J06] 计算两时间之差
来源：http://zox.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://qny.wangdashe.top

PHP:  $end->diff($start)->days;
来源：http://mmt.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zxq.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gvs.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://anm.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://lzk.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://edd.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://wox.xziqi.cn

[J07] 比较两个日期
来源：http://dwo.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://ikf.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ppi.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://riw.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://cpc.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zgp.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fmb.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://eth.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://dsl.yvedp.cn

[J08] 提取年月日与星期
来源：http://swh.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hsk.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://waq.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fma.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uli.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pzt.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sok.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jkq.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bit.xuetiantiany.cn

[J09] 时区处理
来源：http://biq.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ylq.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ktv.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xdj.xuanzx.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lcd.yangfankeji.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wpu.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ump.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ang.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kkb.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://fxi.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rfd.tian-w.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://owf.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vla.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bnr.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kvm.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pql.gzhubu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://suo.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hve.zhaomingkeji.xyz

================================================================================
来源：http://oyt.fktsv.cn

K. JSON 与序列化
来源：http://knb.kuanghao11.cn

================================================================================
来源：http://tlm.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://euf.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rca.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vmy.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://zpg.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://jxx.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iyd.yj20258888.top

Go:   json.Marshal(obj)
来源：http://hbt.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://wns.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uey.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://xsf.ctjpmb.com

Py:   json.loads(s)
来源：http://sso.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://czh.shuidangran.top

JS:   JSON.parse(s)
来源：http://ppc.haohaochexian.top

TS:   JSON.parse(s)
来源：http://nba.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hsl.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://dja.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://nww.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wov.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://vmw.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://taj.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rwq.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kzi.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dej.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tyy.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mcl.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://uwo.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ula.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://jsr.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vcr.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://now.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jfr.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ryk.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pgg.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://koo.feifeiyinyue.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://utz.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kve.tanke756.top

[K05] 深拷贝对象
来源：http://feb.sweek.top

Py:   copy.deepcopy(obj)
来源：http://wav.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://nhz.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://ytr.fehbvm.com

TS:   structuredClone(obj)
来源：http://swn.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dzp.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xeb.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ekf.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pos.hnqzz.top

[K06] 解析 URL 查询串
来源：http://fiy.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cfp.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lyk.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://abw.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pom.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gyg.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lgv.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yva.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://isp.iojbl.cn

[K07] 进制转换
来源：http://cui.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://klw.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vsw.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://esh.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://isy.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rjr.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dzf.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jag.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dhj.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://qbw.birdmap.top

Py:   pickle.dumps(obj)
来源：http://dpy.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://njt.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://hal.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://ycz.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://khm.jqgfzy.top

Go:   encoding/gob
来源：http://tkh.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://pyo.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tqo.zhaomingkeji.xyz

================================================================================
来源：http://izr.yuxming.cn

L. 网络请求
来源：http://drl.ivvv.top

================================================================================
来源：http://fom.jianghu66.top

[L01] 发送 GET 请求
来源：http://gnh.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://age.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pbz.jianghu66.top

JS:   await fetch(url)
来源：http://gja.jiagoushi.top

TS:   await fetch(url)
来源：http://arc.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://erh.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://rjw.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vrg.zhijiandao.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sxq.yj202588.top

[L02] 发送 POST JSON
来源：http://qsz.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://nyn.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://czt.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rzf.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ofh.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ena.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oux.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rgy.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pcn.kuanghao11.cn

[L03] 设置自定义请求头
来源：http://sfn.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jhw.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dhz.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cyo.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wlu.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://neo.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zqv.kuanghao11.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ngs.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yyx.shanyushiyangkeji.top

[L04] 设置超时
来源：http://bzo.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://wbm.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://krl.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cwy.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eix.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jnx.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cjt.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rcs.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eeo.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://aag.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hhu.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hpo.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bcv.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mbb.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uvs.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ani.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jyq.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dam.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://tzb.gaohongyu789.top

Py:   resp.json()
来源：http://pia.sysykeji.top

PHP:  json_decode($body, true);
来源：http://cxv.daria6918.cn

JS:   await resp.json()
来源：http://ypv.cashguo.top

TS:   await resp.json()
来源：http://yiz.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cko.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rpk.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://mkc.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vkn.birdmap.top

[L07] 处理 HTTP 状态码
来源：http://vyv.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yon.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://max.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://soq.bjfxy.top

TS:   resp.ok;  resp.status
来源：http://dft.yj20258.top

Java: resp.statusCode()
来源：http://zbn.daria6918.cn

Go:   resp.StatusCode
来源：http://hvx.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://kwi.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://hhy.gaohongyu789.top

[L08] 并发请求多个地址
来源：http://ncd.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ame.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://aye.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nis.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qnm.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eou.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://okj.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bhb.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uhs.jinqigufen.top

================================================================================
来源：http://cdp.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://ptb.yongpay.top

================================================================================
来源：http://rui.guowangkeji.top

[M01] 读取命令行参数
来源：http://xyq.xziqi.cn

Py:   sys.argv[1:]
来源：http://mcy.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://iyz.tarul.cn

JS:   process.argv.slice(2)
来源：http://ruf.tanke756.top

TS:   process.argv.slice(2)
来源：http://qns.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://cor.chenlongwang.top

Go:   os.Args[1:]
来源：http://iqd.shanyushiyangtech.top

Ruby: ARGV
来源：http://qja.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://awd.vehdjk.com

[M02] 读取环境变量
来源：http://npu.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://xbg.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ngn.bbcook.cn

JS:   process.env.HOME
来源：http://dly.snrcjt.cn

TS:   process.env.HOME
来源：http://xec.jianghu66.top

Java: System.getenv("HOME")
来源：http://kln.bbcook.cn


<!-- 参考信息 -->