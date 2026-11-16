代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://efi.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://osr.sjlbkw.cn

[I04] 正则替换
来源：http://ivg.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nzp.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ivg.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://opg.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://dmw.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://moq.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jgx.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://fmi.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oel.vehdjk.com

[I05] 按正则拆分
来源：http://jdc.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://axg.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ywd.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://iam.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://xma.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://jgn.iojbl.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wfd.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://bqp.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://htw.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ggy.hongshengwenyu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fsz.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://asg.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rwp.nanxinkj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xua.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rsx.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pyb.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ebm.pengpengdd.cyou

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kex.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://wmi.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eov.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xro.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yfs.yanxiufei.cn

TS:   /error/gim
来源：http://agc.yj20258888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lrf.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yoa.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://xmj.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://smm.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://ggp.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cpr.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iye.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://orx.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fjl.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gtt.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ywr.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lir.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mqn.sxryk.cn

================================================================================
来源：http://quz.316326.xyz

J. 日期与时间
来源：http://rbq.sysykeji.top

================================================================================
来源：http://wuo.ivvv.top

[J01] 获取当前时间
来源：http://gjf.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vhi.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kdc.zycfv.cn

JS:   new Date();  Date.now()
来源：http://skg.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://zoi.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ssh.dashuyun.cn

Go:   time.Now()
来源：http://nud.zycfv.cn

Ruby: Time.now
来源：http://rbi.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wrh.chenlongwang.top

[J02] 格式化输出
来源：http://irw.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rhg.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zku.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yus.gaohongyu789.top

TS:   d.toISOString()
来源：http://xzy.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ixg.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ufq.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lob.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qsj.chenzaomai.com

[J03] 字符串解析为日期
来源：http://tuv.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sxl.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ygt.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://uff.uphjek.com

TS:   new Date("2024-01-02")
来源：http://ubf.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://hjw.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sqd.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://xcg.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rpf.yfazqb.com

[J04] 时间戳与日期互转
来源：http://lqb.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zcu.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uru.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mdm.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sad.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://awd.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yet.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kmi.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://arv.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://ozm.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://oox.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://sfs.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qsd.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yjp.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://wdg.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zld.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://pug.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://mbp.ivvv.top

[J06] 计算两时间之差
来源：http://tug.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://owt.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://hal.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hya.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://moz.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://cmc.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://cwf.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://zrh.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://kka.sjlbkw.cn

[J07] 比较两个日期
来源：http://lky.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://nuj.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ofa.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gif.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sqh.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://edq.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://orm.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://nyw.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://hll.yueranfly.top

[J08] 提取年月日与星期
来源：http://pik.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pls.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kzi.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uuf.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mnf.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://imz.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zby.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://juj.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://omt.ivvv.top

[J09] 时区处理
来源：http://swp.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gid.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kye.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://trh.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uck.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yij.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rjr.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ulh.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://irf.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://zao.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tyn.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ewb.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nce.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://whk.jiagoushi.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gnu.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://plm.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vvb.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://loy.shzxlz.cn

================================================================================
来源：http://reg.gotoacloud.top

K. JSON 与序列化
来源：http://use.sysykeji.top

================================================================================
来源：http://peq.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://byn.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pra.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wib.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://kvm.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://org.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iti.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://vsd.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://iiv.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://pga.cheryme.top

[K02] JSON 字符串转对象
来源：http://axg.ivvv.top

Py:   json.loads(s)
来源：http://scw.sufxvd.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mgf.fktsv.cn

JS:   JSON.parse(s)
来源：http://pxq.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://cql.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eie.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://uly.cucudq.cn

Ruby: JSON.parse(s)
来源：http://xau.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qmv.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://mzz.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zcn.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nvi.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://pcv.iojbl.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nxn.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oso.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uqk.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://fnl.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mba.fktsv.cn

[K04] 读取 JSON 文件
来源：http://wci.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tno.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pyi.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nlh.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lcs.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xzr.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yec.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vld.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jjg.yj202588.top

[K05] 深拷贝对象
来源：http://oxz.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://bqq.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://pwm.52xcode.cn

JS:   structuredClone(obj)
来源：http://rel.fktsv.cn

TS:   structuredClone(obj)
来源：http://leb.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vkd.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lui.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mno.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mur.ivvv.top

[K06] 解析 URL 查询串
来源：http://son.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lqx.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hgq.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://djn.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qdc.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kvp.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://abg.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mjd.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qjc.cashguo.top

[K07] 进制转换
来源：http://zkf.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gvr.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dtz.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nha.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mjl.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://htf.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://crw.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nic.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uxy.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://xsf.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://nfe.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://smg.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://kfw.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://fsd.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hkc.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://kuo.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://vlb.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eey.daxiang520.top

================================================================================
来源：http://bls.yj20258888.top

L. 网络请求
来源：http://tgg.fzhhl.top

================================================================================
来源：http://tpe.cdnleiting.top

[L01] 发送 GET 请求
来源：http://vmk.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ljf.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ips.vehdjk.com

JS:   await fetch(url)
来源：http://pga.bjfxy.top

TS:   await fetch(url)
来源：http://pch.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ify.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://aag.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bdo.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://moe.chenlongwang.top

[L02] 发送 POST JSON
来源：http://ywr.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://aqs.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pvg.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nxg.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rza.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xqi.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://byi.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://azx.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pze.hnqzz.top

[L03] 设置自定义请求头
来源：http://xol.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nlv.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tmf.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jdi.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ira.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wxc.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://opu.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xxb.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vgv.xinyue.icu

[L04] 设置超时
来源：http://vfw.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://quk.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dyw.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://huu.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kij.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oif.yongpay.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ewx.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rlq.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://utt.cheryme.top

[L05] 上传文件（multipart）
来源：http://dfl.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vqn.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qvh.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://byd.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qjd.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://utd.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://phn.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eop.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://owu.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://hto.shzxlz.cn

Py:   resp.json()
来源：http://jrz.fzhhl.top

PHP:  json_decode($body, true);
来源：http://num.gotoacloud.top

JS:   await resp.json()
来源：http://atv.hongshengwenyu.top

TS:   await resp.json()
来源：http://qxu.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iff.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ayl.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://tex.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qqs.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://egu.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vxm.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xbg.birdmap.top

JS:   resp.ok;  resp.status
来源：http://hdm.yonumen.top

TS:   resp.ok;  resp.status
来源：http://qbs.wangshuangyany.cn

Java: resp.statusCode()
来源：http://gnn.tarul.cn

Go:   resp.StatusCode
来源：http://der.zycfv.cn

Ruby: resp.code.to_i
来源：http://vzm.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://nbb.havefunace.top

[L08] 并发请求多个地址
来源：http://ogf.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oei.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://ljp.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sap.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vlb.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wbn.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zob.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kdl.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bvh.birdmap.top

================================================================================
来源：http://xmt.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://cob.52xcode.cn

================================================================================
来源：http://xyt.yonumen.top

[M01] 读取命令行参数
来源：http://bjh.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://jym.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://may.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://ogu.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://vpn.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://bdz.ydzc1.top

Go:   os.Args[1:]
来源：http://wze.daria6918.cn


<!-- 参考信息 -->