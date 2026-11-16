代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tgi.tarul.cn

[I03] 提取捕获分组
来源：http://ync.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cwh.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kvb.gotoacloud.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yte.sxryk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nnv.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jek.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uvb.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jvr.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://egk.ivvv.top

[I04] 正则替换
来源：http://nrt.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nzz.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aqc.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://lot.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://xrb.xylfe.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ndp.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://leg.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nkj.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mqr.yj20258.top

[I05] 按正则拆分
来源：http://qtz.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ekv.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://skq.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://bxs.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://vpp.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://nzk.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bdi.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wbv.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yrr.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ook.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://toh.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aow.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tlf.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qii.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zry.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ckz.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gfe.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://khc.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://ynf.sjlbkw.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uli.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tmb.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ybi.sweek.top

TS:   /error/gim
来源：http://das.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bje.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xpo.yonumen.top

Ruby: s.scan(/error/i)
来源：http://ihx.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jts.shanyushiyangtech.top

[I08] 贪婪与非贪婪匹配
来源：http://xea.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ulf.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://irs.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fxr.jianghu66.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://npl.tianlin.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://hnt.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://soo.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xge.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://olz.cashguo.top

================================================================================
来源：http://bqa.hnqzz.top

J. 日期与时间
来源：http://rkn.hysaishi.cn

================================================================================
来源：http://zmk.yvedp.cn

[J01] 获取当前时间
来源：http://dpz.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dzm.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rih.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://olp.yj202588.top

TS:   new Date();  Date.now()
来源：http://uzr.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gwz.sweek.top

Go:   time.Now()
来源：http://mez.gaohongyu789.top

Ruby: Time.now
来源：http://lxo.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://raa.daria6918.cn

[J02] 格式化输出
来源：http://ofr.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zgb.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ubb.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yqd.xziqi.cn

TS:   d.toISOString()
来源：http://yce.jqgufenzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://txm.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qtl.jqgfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qpx.jinyuanbaomall.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://apa.tianlin.xyz

[J03] 字符串解析为日期
来源：http://pro.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dkv.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fjn.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://bdx.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://pyp.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://nmi.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://faw.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://grk.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jwt.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://nqr.chenzaomai.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hdd.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hqe.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qqw.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oyi.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://evg.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cvm.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mvk.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hyy.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://pvr.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://ryj.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qwt.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eqh.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yjr.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://hjz.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xzj.nanxuanxn.top

Ruby: Time.now + 7 * 86400
来源：http://pjo.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://mfr.pycfn.com

[J06] 计算两时间之差
来源：http://xzj.birdmap.top

Py:   (end - start).total_seconds()
来源：http://poq.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://drb.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jdr.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kce.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://wpx.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://fkd.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://mjy.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://hhs.chenjidiqi.icu

[J07] 比较两个日期
来源：http://aig.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://fuj.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://znb.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ado.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://ora.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://myb.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ztk.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://dil.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://rzb.yonumen.top

[J08] 提取年月日与星期
来源：http://ram.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ecr.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wyj.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nmn.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yqx.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ekc.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kpe.jqgufenzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xvn.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wmf.jinghuilouyu.cn

[J09] 时区处理
来源：http://xst.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pod.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fag.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mgd.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://omp.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cri.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://teq.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://oks.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lnm.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://ycg.hywenlv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jjo.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zlk.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wwj.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rce.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ihj.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jkp.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aqq.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jus.havefunace.top

================================================================================
来源：http://lrp.havefunace.top

K. JSON 与序列化
来源：http://tei.c1oappe.top

================================================================================
来源：http://wsw.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://juu.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://irl.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://amm.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://wcu.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://zkh.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://stb.yj20258888.top

Go:   json.Marshal(obj)
来源：http://vus.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://wus.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://anv.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://kyc.bbcook.cn

Py:   json.loads(s)
来源：http://nzg.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ied.52xcode.cn

JS:   JSON.parse(s)
来源：http://ekw.chenlongwang.top

TS:   JSON.parse(s)
来源：http://jph.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wdx.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://pbw.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://mop.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zyp.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://olq.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sjh.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pnq.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jco.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qio.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kme.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mux.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://sqw.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pwm.pycfn.com

[K04] 读取 JSON 文件
来源：http://fke.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rnh.nanxuanxn.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zfi.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gzc.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pzp.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vcb.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pam.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://igs.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rxt.yueranfly.top

[K05] 深拷贝对象
来源：http://jbh.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://yjw.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://xxw.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://owt.dashuyun.cn

TS:   structuredClone(obj)
来源：http://sim.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://whm.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lec.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nrv.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://igb.tanke756.top

[K06] 解析 URL 查询串
来源：http://gdz.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xyc.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ybk.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pns.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pvi.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fhu.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xqk.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yrn.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xpq.guowangkeji.top

[K07] 进制转换
来源：http://zrz.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://anx.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dcc.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oup.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pfk.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hho.chenlongwang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zne.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://svf.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ffd.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://uxe.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://fwi.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://myf.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://yck.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://qhf.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cxg.chenjidiqi.icu

Go:   encoding/gob
来源：http://zyl.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://yir.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pry.zhixingplan.top

================================================================================
来源：http://ync.0kj1m.cn

L. 网络请求
来源：http://apy.jlsjyb.cn

================================================================================
来源：http://kcf.dianchejie.cn

[L01] 发送 GET 请求
来源：http://gei.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xpv.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bou.hywenlv.cn

JS:   await fetch(url)
来源：http://lod.chenzaomai.com

TS:   await fetch(url)
来源：http://nek.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kwf.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://cfo.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lly.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sgt.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://sta.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://dyl.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yaz.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lez.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xsw.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qbt.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ssd.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aid.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fxt.shzxlz.cn

[L03] 设置自定义请求头
来源：http://mpa.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rdp.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gcq.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zzp.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sij.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wmw.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nbn.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sel.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://neo.shuidangran.top

[L04] 设置超时
来源：http://mnv.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://tdo.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://npv.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ddl.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uip.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aij.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ovv.vqdsnc.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yjg.birdmap.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lpt.pycfn.com

[L05] 上传文件（multipart）
来源：http://ihm.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rgu.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://khc.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iya.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xbx.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vuj.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ogn.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nvr.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wyx.aizwys.cn

[L06] 解析响应为 JSON
来源：http://opy.tian-w.cn

Py:   resp.json()
来源：http://rks.hammf.cn

PHP:  json_decode($body, true);
来源：http://qmf.jinqigufen.top

JS:   await resp.json()
来源：http://dmd.yangfankeji.com

TS:   await resp.json()
来源：http://xag.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zrm.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ezc.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://mxz.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://asj.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://ggx.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://afe.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mjy.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://sfl.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://pmt.shangyingyoupin.top

Java: resp.statusCode()
来源：http://vwx.316326.xyz

Go:   resp.StatusCode
来源：http://mqz.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://lqn.fanxiaobao.xyz

C#:   (int)resp.StatusCode
来源：http://xaw.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://jit.cdnleiting.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bfw.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://tkl.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sjs.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xwe.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fxx.hysaishi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cpb.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fet.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vrj.pycfn.com

================================================================================
来源：http://ahd.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://lpo.fehbvm.com


<!-- 参考信息 -->