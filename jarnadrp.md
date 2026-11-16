代发 wailian999

TS:   s.match(/\d+/g)
来源：http://cqv.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qtr.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vjt.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://tpr.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ioi.hesvh.cn

[I03] 提取捕获分组
来源：http://jdz.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ooe.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vjn.dianchejie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qez.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xkl.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tty.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gxk.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pet.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gbw.zhengqikj.top

[I04] 正则替换
来源：http://qkk.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ejf.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wil.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hnx.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://nsl.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://rbw.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iot.yuxming.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eyf.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://agb.dashuyun.cn

[I05] 按正则拆分
来源：http://wfy.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ryw.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ydt.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://igq.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://uqh.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://pst.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://znk.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rsx.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rvb.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cfk.hywenlv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vpo.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sxn.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zjy.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jxu.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uhr.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wod.gotoacloud.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zmo.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qmj.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://dgn.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yxh.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hhe.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zoj.daria6918.cn

TS:   /error/gim
来源：http://oqx.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bje.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ivz.pycfn.com

Ruby: s.scan(/error/i)
来源：http://oit.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vqk.pycfn.com

[I08] 贪婪与非贪婪匹配
来源：http://mao.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oeq.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ztu.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ykr.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://goz.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mlw.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gsd.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mdz.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qxj.hysaishi.cn

================================================================================
来源：http://cdo.iojbl.cn

J. 日期与时间
来源：http://vcq.jiagoushi.top

================================================================================
来源：http://yrm.ydjk.org.cn

[J01] 获取当前时间
来源：http://soe.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ajp.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dlm.yuxming.cn

JS:   new Date();  Date.now()
来源：http://uey.hcnkem.com

TS:   new Date();  Date.now()
来源：http://ugh.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wmx.jqgfzy.top

Go:   time.Now()
来源：http://iqr.shzxlz.cn

Ruby: Time.now
来源：http://sef.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jbl.sufxvd.cn

[J02] 格式化输出
来源：http://izo.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://phb.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cmr.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://loa.52xcode.cn

TS:   d.toISOString()
来源：http://mgh.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fri.jianghu66.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hnd.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ses.mhx1999.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://twq.yj20258.top

[J03] 字符串解析为日期
来源：http://chi.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xob.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zti.yongpay.top

JS:   new Date("2024-01-02")
来源：http://xmu.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://lhl.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zha.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vmf.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://oud.yangfankeji.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://neb.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://hry.yangfankeji.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cri.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eqf.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jpp.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xfe.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mpj.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://khr.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nez.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://myf.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://ojr.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://qpf.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pul.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qzx.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ric.tarul.cn

Java: LocalDate.now().plusDays(7)
来源：http://ibn.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cdo.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://pca.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rrb.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://whv.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://umh.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://pir.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rzj.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nrt.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ybt.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://xmn.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://xhy.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://vmp.dianchejie.cn

[J07] 比较两个日期
来源：http://raj.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://jaa.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bzq.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://rus.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zgj.uphjek.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sxo.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ssi.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zuh.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://vox.zhengqikj.top

[J08] 提取年月日与星期
来源：http://utr.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wxa.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kmi.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mgj.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uhj.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iql.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jvq.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bnu.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://whb.gotoacloud.top

[J09] 时区处理
来源：http://oxd.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tmw.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aqs.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://abh.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://str.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://joi.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lor.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bje.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jnd.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://urg.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cix.hnqzz.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mbt.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lvx.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ahx.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sut.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tbg.hnxiangtu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bvs.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mau.bbcook.cn

================================================================================
来源：http://iaw.jyoumei.cn

K. JSON 与序列化
来源：http://ygx.dashuyun.cn

================================================================================
来源：http://qpn.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://zzi.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lbp.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ooe.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://oxh.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://bpk.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ggn.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://vsp.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://psc.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lis.uphjek.com

[K02] JSON 字符串转对象
来源：http://hpu.hongshengwenyu.top

Py:   json.loads(s)
来源：http://wbz.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://akp.zdqjudy.top

JS:   JSON.parse(s)
来源：http://ngu.cashguo.top

TS:   JSON.parse(s)
来源：http://gac.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sxm.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://pmd.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://lbl.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nqq.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://zmw.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bfg.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rja.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://wjm.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://hjg.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wax.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kyj.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aon.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jhi.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://ykm.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hfk.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pom.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nrc.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dtc.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://scy.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gzo.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mmr.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://snp.cashguo.top

[K05] 深拷贝对象
来源：http://bro.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://dtg.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://ijz.haohaochexian.top

JS:   structuredClone(obj)
来源：http://pzk.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://djp.jiagoushi.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ecw.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kwk.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gsu.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rkl.52xcode.cn

[K06] 解析 URL 查询串
来源：http://wma.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gtq.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://grx.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ykh.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hni.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ear.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://flr.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pxa.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zlq.smart0.xyz

[K07] 进制转换
来源：http://rbf.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tff.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mty.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iuq.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uko.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fpw.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bgr.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gzq.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sry.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://ldy.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://qkj.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mhb.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://lcj.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://qwh.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vhs.zhoulong.xyz

Go:   encoding/gob
来源：http://shq.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://zxv.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rcj.yongpay.top

================================================================================
来源：http://din.zdqjudy.top

L. 网络请求
来源：http://gag.cashguo.top

================================================================================
来源：http://ejh.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://wzl.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://csp.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vvo.pengpengdd.cyou

JS:   await fetch(url)
来源：http://qzr.guannengcc.top

TS:   await fetch(url)
来源：http://xvo.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://enw.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://ehp.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ada.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://isg.hywenlv.cn

[L02] 发送 POST JSON
来源：http://zoc.xziqi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yyw.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mig.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rbu.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rgr.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dao.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://owk.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ayg.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xgp.yj20258.top

[L03] 设置自定义请求头
来源：http://ycy.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yux.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ofy.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fwp.jiagoushi.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bsg.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mgm.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://moy.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ylp.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tvs.cdnleiting.top

[L04] 设置超时
来源：http://ndn.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://ell.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://umv.yfazqb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://izi.ehwqpu.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zbq.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mjx.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gis.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bss.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nry.vehdjk.com

[L05] 上传文件（multipart）
来源：http://ydw.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wnr.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yjc.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jfr.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bip.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://etb.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tuw.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rtc.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uun.bjfxy.top

[L06] 解析响应为 JSON
来源：http://cms.jinqigufen.top

Py:   resp.json()
来源：http://wxv.nwbrower.top

PHP:  json_decode($body, true);
来源：http://edt.jinqigfzy.top

JS:   await resp.json()
来源：http://ysh.hesvh.cn

TS:   await resp.json()
来源：http://gso.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ank.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xqg.hnxiangtu.top

Ruby: JSON.parse(resp.body)
来源：http://oxt.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lne.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://btn.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jwp.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jen.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://jei.yj202588.top

TS:   resp.ok;  resp.status
来源：http://ufe.gaohongyu789.top

Java: resp.statusCode()
来源：http://kaw.smart0.xyz

Go:   resp.StatusCode
来源：http://uth.ybcxt.top

Ruby: resp.code.to_i
来源：http://mgx.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://luj.jiagoushi.top

[L08] 并发请求多个地址
来源：http://yqr.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nub.zdbjq.cn

PHP:  curl_multi_init() 系列
来源：http://cbj.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cfq.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://anx.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sep.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fkd.bjfxy.top


<!-- 参考信息 -->