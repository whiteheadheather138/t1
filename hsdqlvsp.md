代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ykq.jqgfzy.top

[I03] 提取捕获分组
来源：http://fdp.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://owc.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://skb.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lxw.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ngj.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cqc.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://csc.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zyy.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wxv.guannengcc.top

[I04] 正则替换
来源：http://pam.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rgj.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cih.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://qhe.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://ldb.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lji.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://hec.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pdw.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iiy.yuanzhike.top

[I05] 按正则拆分
来源：http://dno.fktsv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://szh.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://utd.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://prb.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://spd.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://fyv.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pgj.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://unq.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bow.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aom.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ybq.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://igy.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hie.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pcd.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jgm.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ikc.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eqa.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://btz.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://ods.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lff.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cht.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ppj.chenjidiqi.icu

TS:   /error/gim
来源：http://iug.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pcb.xuetiantiany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zzl.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://vrm.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ynd.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://nhw.chenlongwang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vkp.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xfa.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eso.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rfw.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ftu.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rdz.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cwp.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ihp.fzhhl.top

================================================================================
来源：http://rqj.hfpthk.cn

J. 日期与时间
来源：http://xen.yj202588.top

================================================================================
来源：http://fup.tarul.cn

[J01] 获取当前时间
来源：http://ksa.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://orh.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ynf.gzhubu.top

JS:   new Date();  Date.now()
来源：http://top.wangdashe.top

TS:   new Date();  Date.now()
来源：http://pyl.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tfb.meibo888.top

Go:   time.Now()
来源：http://irp.xylfe.cn

Ruby: Time.now
来源：http://lva.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jwi.yj202588.top

[J02] 格式化输出
来源：http://qck.yonumen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gme.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sal.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nmy.guannengcc.top

TS:   d.toISOString()
来源：http://clu.jqgufenzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ggi.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://key.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yyd.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tlc.hcnkem.com

[J03] 字符串解析为日期
来源：http://cxp.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ith.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iau.yvedp.cn

JS:   new Date("2024-01-02")
来源：http://fxd.zhongyouzk.top

TS:   new Date("2024-01-02")
来源：http://kzz.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://umy.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cxr.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://lor.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://epn.daria6918.cn

[J04] 时间戳与日期互转
来源：http://vwb.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bbk.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mqt.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://clo.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://byp.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cvi.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://inv.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tiw.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://usy.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://qlv.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://rqs.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xxx.ppjwa.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://txm.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cya.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://vzs.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ojx.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://tdi.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://ufj.zdbjq.cn

[J06] 计算两时间之差
来源：http://fyl.sjlbkw.cn

Py:   (end - start).total_seconds()
来源：http://slx.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://xhd.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uin.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://urd.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://ehx.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://nrz.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://njs.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://trv.bbcook.cn

[J07] 比较两个日期
来源：http://lji.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://srq.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ffh.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://owi.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://utt.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dhh.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aqj.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://dqw.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://exr.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://trl.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ynj.sweek.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://aim.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dwi.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bbl.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bbu.jyoumei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://axl.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hon.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xpo.jinqigufen.top

[J09] 时区处理
来源：http://wly.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ltn.zhiwuduotai.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lfd.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wot.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://njq.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ids.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://esz.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mrx.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pom.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://ikp.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kdz.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hzy.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gkh.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://efo.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rxp.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://frg.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fny.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aey.316326.xyz

================================================================================
来源：http://kxh.nanxuanxn.top

K. JSON 与序列化
来源：http://yoo.meibo888.top

================================================================================
来源：http://mfc.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://jmh.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kaj.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cyf.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://iyq.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://des.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sbj.birdmap.top

Go:   json.Marshal(obj)
来源：http://zdg.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://sgj.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dom.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://xbt.sweek.top

Py:   json.loads(s)
来源：http://dun.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lwk.cucudq.cn

JS:   JSON.parse(s)
来源：http://uyn.aibaodan.cn

TS:   JSON.parse(s)
来源：http://ekx.pengpengdd.cyou

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cac.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://jtm.316326.xyz

Ruby: JSON.parse(s)
来源：http://fep.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sez.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://ywo.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bmn.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://laj.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bgc.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dsx.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qiq.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mfp.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zff.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://anv.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://buu.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rny.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dbo.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rrj.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://khq.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mpo.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sew.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://odv.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jpy.redwolf501.top

[K05] 深拷贝对象
来源：http://ypp.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://gqp.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://kcb.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://jgh.pycfn.com

TS:   structuredClone(obj)
来源：http://akd.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://amt.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://trv.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://icd.daria6918.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zus.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://pgs.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tfb.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rbx.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://edq.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://grn.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tqx.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wsv.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hqa.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fxp.dashuyun.cn

[K07] 进制转换
来源：http://sez.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fdh.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://doj.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aga.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lbm.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cih.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uvr.cdnleiting.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cpi.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dxx.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://mod.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://oki.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://voj.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://ztd.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://zoj.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sla.sufxvd.cn

Go:   encoding/gob
来源：http://xdu.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://acq.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yhp.daria6918.cn

================================================================================
来源：http://ejx.daxiang520.top

L. 网络请求
来源：http://jea.zhiwuduotai.top

================================================================================
来源：http://sjs.zycfv.cn

[L01] 发送 GET 请求
来源：http://oog.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ldm.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bvq.dashuyun.cn

JS:   await fetch(url)
来源：http://bhr.tian-w.cn

TS:   await fetch(url)
来源：http://ugh.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ydq.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://tey.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bku.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://scn.vehdjk.com

[L02] 发送 POST JSON
来源：http://jlp.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cvg.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wnq.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aye.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nsr.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://spt.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ktj.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ven.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wbq.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://rbr.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://izg.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oyk.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bpc.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://skw.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nzw.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uef.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://frx.tarul.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mxs.jinqigufen.top

[L04] 设置超时
来源：http://gwx.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://qkh.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tnr.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wxk.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wed.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zbi.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zyf.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cdf.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uod.xziqi.cn

[L05] 上传文件（multipart）
来源：http://fku.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nga.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tql.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qvg.yonumen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sjc.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ikz.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fvy.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lse.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pmp.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://ded.sjlbkw.cn

Py:   resp.json()
来源：http://mll.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://imp.nwbrower.top

JS:   await resp.json()
来源：http://zkn.yvedp.cn

TS:   await resp.json()
来源：http://afk.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ysf.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dea.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://ndv.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fau.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://kfw.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qtm.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nzz.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://fpy.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://jhq.xinyue.icu

Java: resp.statusCode()
来源：http://gyl.shzxlz.cn

Go:   resp.StatusCode
来源：http://qmw.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://iuv.pengpengdd.cyou

C#:   (int)resp.StatusCode
来源：http://mqv.ydjk.org.cn

[L08] 并发请求多个地址
来源：http://and.ybcxt.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cdv.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://sxy.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zrm.quarkkingdee.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hmg.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lus.yj202588.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pvc.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hfg.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tzl.jqgufenzy.top

================================================================================
来源：http://vqq.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://lby.nwbrower.top


<!-- 参考信息 -->