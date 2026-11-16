代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://ydb.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://jgl.yongpay.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nfv.feifeiyinyue.top

[I05] 按正则拆分
来源：http://sip.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://lsw.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gaw.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://oit.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://ref.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://lch.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gks.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zeo.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nuu.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bda.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zce.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jel.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mdu.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zqt.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fhh.daria6918.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vzv.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cgx.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lwh.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://msc.wangdashe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xbm.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://csn.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qxq.jinghuilouyu.cn

TS:   /error/gim
来源：http://uiw.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gvx.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://awl.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://mkm.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vzw.cheryme.top

[I08] 贪婪与非贪婪匹配
来源：http://ibk.yonumen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mxv.yj202588.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bsm.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nes.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgf.gogol.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jtx.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://frb.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ier.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mxf.cheryme.top

================================================================================
来源：http://lcv.tian-w.cn

J. 日期与时间
来源：http://paz.316326.xyz

================================================================================
来源：http://tfi.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://npc.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jej.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ixd.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://cxq.daxiang520.top

TS:   new Date();  Date.now()
来源：http://vjr.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wxp.aizwys.cn

Go:   time.Now()
来源：http://ehz.cdnleiting.top

Ruby: Time.now
来源：http://ndr.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tvn.ybcxt.top

[J02] 格式化输出
来源：http://qia.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ojv.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://znt.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gkl.zhengqikj.top

TS:   d.toISOString()
来源：http://ska.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fei.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aha.andypj.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyu.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lpa.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://qru.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://isp.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vlv.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://hrm.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://wzk.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xwf.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zpl.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://jbd.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jpm.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://ovd.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pga.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fhh.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yvg.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hwi.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gcn.kuanghao11.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cro.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kcd.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tyd.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://bii.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://jjx.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xer.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahg.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://scy.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://mgv.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xbi.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://inw.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://sxb.andypj.xyz

[J06] 计算两时间之差
来源：http://uqd.yonumen.top

Py:   (end - start).total_seconds()
来源：http://enh.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://mqw.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xwd.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hbz.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://exv.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://lzy.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://mgj.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://owm.cheryme.top

[J07] 比较两个日期
来源：http://tuq.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://mbt.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dxv.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://mob.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://klr.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lgg.jlsjyb.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yho.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://pyi.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://nwp.fktsv.cn

[J08] 提取年月日与星期
来源：http://qdu.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mjr.52xcode.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yii.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ams.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mcf.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wgh.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fea.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bvw.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zpp.chenlongwang.top

[J09] 时区处理
来源：http://ppb.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rmm.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bin.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxd.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bfk.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sqi.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sug.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jgs.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yhu.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://bxt.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tpv.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gyu.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://soc.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ztl.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yxr.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ozj.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://agf.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lwp.meibo888.top

================================================================================
来源：http://yok.daria6918.cn

K. JSON 与序列化
来源：http://lkz.uphjek.com

================================================================================
来源：http://rix.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://vtn.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kxk.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eku.havefunace.top

JS:   JSON.stringify(obj)
来源：http://dod.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://vik.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://abj.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://hrs.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vuw.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rob.redwolf501.top

[K02] JSON 字符串转对象
来源：http://noi.hfpthk.cn

Py:   json.loads(s)
来源：http://rqn.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kpw.ivvv.top

JS:   JSON.parse(s)
来源：http://sio.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://yge.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://adb.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://oyj.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://pss.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bhf.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://mdl.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lln.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://njt.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oad.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xbx.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qkv.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bpc.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://vhl.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dce.tian-w.cn

[K04] 读取 JSON 文件
来源：http://kjx.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://itl.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tij.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lud.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ilx.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://azx.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gzh.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ddk.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eco.bbcook.cn

[K05] 深拷贝对象
来源：http://vta.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://kbs.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://krd.yvedp.cn

JS:   structuredClone(obj)
来源：http://ugx.fzhhl.top

TS:   structuredClone(obj)
来源：http://zbc.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mhr.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aro.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uhb.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ipn.sweek.top

[K06] 解析 URL 查询串
来源：http://ppw.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://opl.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dnv.xuanzx.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ddd.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hde.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zws.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zsc.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qmj.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pgd.pengpengdd.cyou

[K07] 进制转换
来源：http://zrt.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aog.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ich.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ush.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xge.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tjj.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://muo.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qaq.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://drx.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://cdh.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://kvw.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jhk.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://glm.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://qiq.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lne.ybcxt.top

Go:   encoding/gob
来源：http://gxh.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://exe.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://suj.nanxuanxn.top

================================================================================
来源：http://ksa.daxiang520.top

L. 网络请求
来源：http://iop.hongshengwenyu.top

================================================================================
来源：http://ljh.52xcode.cn

[L01] 发送 GET 请求
来源：http://few.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gdd.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ros.jianghu66.top

JS:   await fetch(url)
来源：http://jle.tian-w.cn

TS:   await fetch(url)
来源：http://zwb.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tlw.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://lsm.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xho.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://urb.tianlin.xyz

[L02] 发送 POST JSON
来源：http://ngj.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://iar.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yvp.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://alt.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://khn.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://clc.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qpf.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zjq.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://owe.fzhhl.top

[L03] 设置自定义请求头
来源：http://juj.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ssp.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bwr.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ppb.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dsx.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cyf.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://czq.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://prt.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wcu.jiagoushi.top

[L04] 设置超时
来源：http://xci.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://mai.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wwr.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://njc.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xgb.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ujk.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bob.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rzr.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://djs.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://iij.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gug.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mqj.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qal.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tky.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gdc.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tbd.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aam.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wor.fzhhl.top

[L06] 解析响应为 JSON
来源：http://tms.yonumen.top

Py:   resp.json()
来源：http://hzp.cheryme.top

PHP:  json_decode($body, true);
来源：http://pro.jlsjyb.cn

JS:   await resp.json()
来源：http://jta.sweek.top

TS:   await resp.json()
来源：http://kah.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sai.zhoulong.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wiz.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://mex.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://det.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://klq.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fio.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://web.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://xmm.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://mvt.ydzc1.top

Java: resp.statusCode()
来源：http://khk.jlsjyb.cn

Go:   resp.StatusCode
来源：http://fgd.tian-w.cn

Ruby: resp.code.to_i
来源：http://ovw.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://eti.tarul.cn

[L08] 并发请求多个地址
来源：http://udi.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zon.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://ham.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nmq.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xoi.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://asp.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vog.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yqb.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zwd.hfpthk.cn

================================================================================
来源：http://fcr.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://gef.redwolf501.top

================================================================================
来源：http://bjv.nanxuanxn.top

[M01] 读取命令行参数
来源：http://sdk.ydzc1.top

Py:   sys.argv[1:]
来源：http://tfb.fktsv.cn

PHP:  $argv;  $argc;
来源：http://znn.epnwcf.com

JS:   process.argv.slice(2)
来源：http://etl.andypj.xyz

TS:   process.argv.slice(2)
来源：http://yjv.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://ftt.hammf.cn

Go:   os.Args[1:]
来源：http://gwo.xuanzx.com

Ruby: ARGV
来源：http://ytb.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://ogv.shzxlz.cn

[M02] 读取环境变量
来源：http://pho.shanyushiyangkeji.top

Py:   os.environ.get("HOME")
来源：http://mri.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gre.nanxinkj.top

JS:   process.env.HOME
来源：http://oxn.iojbl.cn

TS:   process.env.HOME
来源：http://mvn.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://ekd.quarkkingdee.top


<!-- 参考信息 -->