代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gwi.pengpengdd.cyou

[I03] 提取捕获分组
来源：http://rfi.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bwm.chenzaomai.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://amx.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://asn.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://msw.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oea.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qhi.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sin.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nku.ehwqpu.com

[I04] 正则替换
来源：http://tmh.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hew.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cla.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://pwz.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://vyp.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://uup.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wxw.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kqf.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ifm.jqgfzy.top

[I05] 按正则拆分
来源：http://esg.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://buo.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hcc.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://yem.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://goh.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://zwr.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vzr.guannengcc.top

Ruby: s.split(/\s*,\s*/)
来源：http://sni.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zan.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mag.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fxm.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vyr.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qwl.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lyi.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://exi.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mdw.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bbe.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oji.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://uxe.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rpm.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dte.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://owu.tianlin.xyz

TS:   /error/gim
来源：http://dfz.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fzu.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vls.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://xar.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zfm.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://mmw.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pni.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://elj.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cqj.zhongyouzk.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pyj.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oxh.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bic.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qdj.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jnw.mhx1999.top

================================================================================
来源：http://xap.xinyue.icu

J. 日期与时间
来源：http://ypr.nanxuanxn.top

================================================================================
来源：http://aen.chenzaomai.com

[J01] 获取当前时间
来源：http://ypx.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xmj.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://djt.mhx1999.top

JS:   new Date();  Date.now()
来源：http://lhh.ybcxt.top

TS:   new Date();  Date.now()
来源：http://cjn.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://glh.havefunace.top

Go:   time.Now()
来源：http://goe.tanke756.top

Ruby: Time.now
来源：http://dsz.xziqi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hnr.epnwcf.com

[J02] 格式化输出
来源：http://oew.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qzl.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kee.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wdq.nwbrower.top

TS:   d.toISOString()
来源：http://mlm.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bbg.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://umv.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kov.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hee.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://crb.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ngy.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://srl.tanke756.top

JS:   new Date("2024-01-02")
来源：http://gfa.zhongyouzk.top

TS:   new Date("2024-01-02")
来源：http://qkr.cucudq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://giw.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://coc.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://oxl.zhongyouzk.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fib.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://xtf.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xxh.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lso.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lsq.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://utr.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lxy.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://own.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zmd.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qtv.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://hts.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://soi.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wbx.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lmr.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qxc.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://jpf.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://htg.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://liy.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://iss.sxryk.cn

[J06] 计算两时间之差
来源：http://neb.0kj1m.cn

Py:   (end - start).total_seconds()
来源：http://ngw.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://smo.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://btx.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jfv.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://sgv.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://ewc.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://iys.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://jzh.andypj.xyz

[J07] 比较两个日期
来源：http://ret.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://mzn.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cej.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://jcw.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sxc.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ygs.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fiw.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://bdh.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://lvw.fehbvm.com

[J08] 提取年月日与星期
来源：http://xvh.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jhi.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cfi.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jyt.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cjt.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vsp.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uve.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mxa.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bdm.daria6918.cn

[J09] 时区处理
来源：http://pmi.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ujm.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sbw.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kzn.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fvg.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cot.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oyk.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qup.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mpu.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://itw.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bmh.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://end.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wuu.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kpp.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nda.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lgf.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gva.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://agx.bbcook.cn

================================================================================
来源：http://ajo.xinyue.icu

K. JSON 与序列化
来源：http://tsk.316326.xyz

================================================================================
来源：http://jzv.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://hqh.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xtq.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vst.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://izh.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://fom.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zqv.xziqi.cn

Go:   json.Marshal(obj)
来源：http://xzu.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gei.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fak.redwolf501.top

[K02] JSON 字符串转对象
来源：http://jre.bjfxy.top

Py:   json.loads(s)
来源：http://seo.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://paj.tian-w.cn

JS:   JSON.parse(s)
来源：http://wky.bjfxy.top

TS:   JSON.parse(s)
来源：http://ikk.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mwe.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://xcj.daria6918.cn

Ruby: JSON.parse(s)
来源：http://ckd.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://swy.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://nyt.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://udl.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gyj.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://icy.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jxq.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sea.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dem.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://enj.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oou.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://gow.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wtr.dianchejie.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rvy.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zhe.52xcode.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://glm.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hnh.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sji.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jrs.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hld.iojbl.cn

[K05] 深拷贝对象
来源：http://qwv.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://kvs.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://bgk.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://mqc.smart0.xyz

TS:   structuredClone(obj)
来源：http://sic.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tnv.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bfp.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ozf.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hmt.yvedp.cn

[K06] 解析 URL 查询串
来源：http://qvp.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ufl.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cvb.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tud.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xtg.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gen.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://nkx.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lfv.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xnf.9152youxi.cn

[K07] 进制转换
来源：http://rvq.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wyt.yonumen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tzs.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mdh.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qmm.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lux.ywan-chungtsiang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tnj.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oes.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eer.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://lbp.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://hve.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ioj.yueranfly.top

JS:   v8.serialize(obj)        // Node
来源：http://che.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://faf.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://isd.316326.xyz

Go:   encoding/gob
来源：http://gid.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://wfh.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zkf.cdnleiting.top

================================================================================
来源：http://ael.wangdashe.top

L. 网络请求
来源：http://qrl.cheryme.top

================================================================================
来源：http://cqx.fzhhl.top

[L01] 发送 GET 请求
来源：http://pfq.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ewc.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jpx.quarkkingdee.top

JS:   await fetch(url)
来源：http://arz.9152youxi.cn

TS:   await fetch(url)
来源：http://pby.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ihi.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://hvw.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wkf.sxryk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zzo.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://oyb.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://kgy.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://anm.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ahj.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xva.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wfw.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://azj.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lps.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ipe.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://uko.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qol.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qzk.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wtc.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zmr.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ohx.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jyy.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ksm.tianlin.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tvx.quarkkingdee.top

[L04] 设置超时
来源：http://obl.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://tux.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tbd.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ojp.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://txf.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kcq.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hxd.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ieb.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gvx.andypj.xyz

[L05] 上传文件（multipart）
来源：http://sul.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cyx.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://thr.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eos.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wgq.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://air.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://giy.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://scv.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rvo.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://aep.yongpay.top

Py:   resp.json()
来源：http://pns.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://vwz.sufxvd.cn

JS:   await resp.json()
来源：http://mja.zdbjq.cn

TS:   await resp.json()
来源：http://ccx.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vny.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ipb.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://lox.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lrq.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://pbh.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zer.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://skt.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://dxr.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://hxb.tarul.cn

Java: resp.statusCode()
来源：http://npx.hesvh.cn

Go:   resp.StatusCode
来源：http://qah.yuanzhike.top

Ruby: resp.code.to_i
来源：http://pch.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://nuk.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://bcg.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yai.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://eob.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cjn.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bmc.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wqh.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pjt.cheryme.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uvs.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ccx.xuetiantiany.cn

================================================================================
来源：http://dqp.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://mjd.ydzc1.top


<!-- 参考信息 -->