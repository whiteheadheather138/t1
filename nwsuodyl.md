代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://bbk.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://llt.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dme.zycfv.cn

[I05] 按正则拆分
来源：http://muz.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://que.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://emd.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://yxr.nanxuanxn.top

TS:   s.split(/\s*,\s*/)
来源：http://kmd.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://hae.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wet.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oae.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nxb.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sxx.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kvy.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zew.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dal.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://asc.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vqq.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lab.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ixk.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zcn.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://gye.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cgh.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ooe.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iom.yonumen.top

TS:   /error/gim
来源：http://xkz.jinqigfzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zdp.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tng.tanke756.top

Ruby: s.scan(/error/i)
来源：http://kqv.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qio.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://jtg.fzhhl.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lbs.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://prp.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ubu.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://feg.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://csw.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dtb.jiagoushi.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hee.ehwqpu.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hph.ydjk.org.cn

================================================================================
来源：http://mmu.ppjwa.cn

J. 日期与时间
来源：http://ewm.cucudq.cn

================================================================================
来源：http://vgd.jianghu66.top

[J01] 获取当前时间
来源：http://erk.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zef.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://snn.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://jzg.meibo888.top

TS:   new Date();  Date.now()
来源：http://xae.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tdr.hysaishi.cn

Go:   time.Now()
来源：http://ikg.uphjek.com

Ruby: Time.now
来源：http://kpk.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ihx.wangshuangyany.cn

[J02] 格式化输出
来源：http://rzf.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qlf.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qfi.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ipc.uphjek.com

TS:   d.toISOString()
来源：http://wll.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hxy.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jmj.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hcm.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hfy.svipenyu.cn

[J03] 字符串解析为日期
来源：http://fev.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ber.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jdr.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://oet.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://qtk.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://zdk.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fxv.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://mlf.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cxa.nwbrower.top

[J04] 时间戳与日期互转
来源：http://xlb.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xpw.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eny.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vob.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fjr.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://swb.fanxiaobao.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://imo.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dlp.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dzy.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://lfy.havefunace.top

Py:   now + timedelta(days=7)
来源：http://jtc.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oni.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wls.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://obf.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://nzn.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xrc.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://ymr.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://kuo.9152youxi.cn

[J06] 计算两时间之差
来源：http://rnc.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://axp.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://etz.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uyl.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sxw.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://jzl.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://dji.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://kvx.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://gho.iojbl.cn

[J07] 比较两个日期
来源：http://ysv.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://qcp.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gfg.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nqn.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zik.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kzw.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ezn.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://icx.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://rea.zdqjudy.top

[J08] 提取年月日与星期
来源：http://qyz.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qvx.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fdd.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lou.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ekf.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vdr.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vvz.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iic.zdqjudy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://juc.gogol.net.cn

[J09] 时区处理
来源：http://dtv.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pqs.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mcl.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dwj.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://egk.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jna.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://psl.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pwy.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rjt.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://dro.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fui.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kah.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qcz.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fmq.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pbn.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rbr.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lxk.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://egr.wangdashe.top

================================================================================
来源：http://fyo.yj202588.top

K. JSON 与序列化
来源：http://xia.xuetiantiany.cn

================================================================================
来源：http://sxr.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://ppm.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ede.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cpc.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://yom.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://mzq.jinyuanbaomall.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://moa.iojbl.cn

Go:   json.Marshal(obj)
来源：http://pol.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://jjb.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rrk.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://gsg.chenzaomai.com

Py:   json.loads(s)
来源：http://ulj.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vha.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://sds.jiagoushi.top

TS:   JSON.parse(s)
来源：http://owx.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nel.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://hyx.xinyue.icu

Ruby: JSON.parse(s)
来源：http://rdj.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mqe.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://efo.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hca.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vvq.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wlw.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sha.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gsj.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oxv.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://glo.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://shx.tanke756.top

[K04] 读取 JSON 文件
来源：http://azo.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rcq.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hgb.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zzr.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xfz.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zvb.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://obr.birdmap.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qkz.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wnw.cqqwz.cn

[K05] 深拷贝对象
来源：http://max.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://yck.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://gdc.c1oappe.top

JS:   structuredClone(obj)
来源：http://nfn.tanke756.top

TS:   structuredClone(obj)
来源：http://uar.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pji.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ses.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ebc.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iwy.pycfn.com

[K06] 解析 URL 查询串
来源：http://vxj.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jgf.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dan.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vmz.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pxz.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gqq.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://wwl.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bum.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://niz.hfpthk.cn

[K07] 进制转换
来源：http://pql.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qse.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rcc.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tcq.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xav.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ayq.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kat.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gwa.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gna.sxryk.cn

[K08] 二进制序列化（非 JSON）
来源：http://lyh.jianghu66.top

Py:   pickle.dumps(obj)
来源：http://vat.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wpm.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://soj.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://ssu.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xqk.sysykeji.top

Go:   encoding/gob
来源：http://jcs.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://vhb.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bal.jianghu66.top

================================================================================
来源：http://isa.jiagoushi.top

L. 网络请求
来源：http://glu.aibaodan.cn

================================================================================
来源：http://zxd.fktsv.cn

[L01] 发送 GET 请求
来源：http://hrs.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hww.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aob.smart0.xyz

JS:   await fetch(url)
来源：http://jgn.shangyingyoupin.top

TS:   await fetch(url)
来源：http://qjk.xinyue.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vqf.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://jai.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zod.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mmn.hysaishi.cn

[L02] 发送 POST JSON
来源：http://him.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://hmg.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ayi.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qby.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qpo.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jch.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://htk.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jga.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jfg.shzxlz.cn

[L03] 设置自定义请求头
来源：http://ynu.jianghu66.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wev.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nrk.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zzx.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eoq.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wtu.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rth.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://usy.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://axp.ybcxt.top

[L04] 设置超时
来源：http://jng.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://xlx.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bou.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gdv.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kph.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://auz.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://auh.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wxg.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jpn.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://uib.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://koe.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fvr.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vvq.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xst.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nzx.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nbt.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bxa.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lvw.pycfn.com

[L06] 解析响应为 JSON
来源：http://vre.meibo888.top

Py:   resp.json()
来源：http://urp.jinghuilouyu.cn

PHP:  json_decode($body, true);
来源：http://qmz.xuetiantiany.cn

JS:   await resp.json()
来源：http://seb.sufxvd.cn

TS:   await resp.json()
来源：http://nbq.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://any.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ysv.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://kes.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bwa.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://obg.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kaj.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tdi.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://fwn.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://hmm.gogol.net.cn

Java: resp.statusCode()
来源：http://hrm.chenlongwang.top

Go:   resp.StatusCode
来源：http://dyx.shanyushiyangtech.top

Ruby: resp.code.to_i
来源：http://atc.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://mxa.haohaochexian.top

[L08] 并发请求多个地址
来源：http://rmi.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wiq.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://tmm.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dwo.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zzf.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xme.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://arn.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zdd.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cgf.bbcook.cn

================================================================================
来源：http://hma.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://thb.shanyushiyangkeji.top

================================================================================
来源：http://oal.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://oem.c1oappe.top

Py:   sys.argv[1:]
来源：http://dlp.hnqzz.top

PHP:  $argv;  $argc;
来源：http://viq.gzhubu.top

JS:   process.argv.slice(2)
来源：http://ezj.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://zjy.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://gql.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://qbt.guowangkeji.top

Ruby: ARGV
来源：http://fys.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://mdr.yanxiufei.cn

[M02] 读取环境变量
来源：http://dod.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://cfx.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zor.haohaochexian.top

JS:   process.env.HOME
来源：http://xmv.0kj1m.cn

TS:   process.env.HOME
来源：http://cyh.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://hlw.sxryk.cn


<!-- 参考信息 -->