代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qle.haohaochexian.top

[I03] 提取捕获分组
来源：http://bwu.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iyr.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nfi.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ltx.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rxb.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://exw.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xgx.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qcb.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tmx.meibo888.top

[I04] 正则替换
来源：http://tqw.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zgd.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gus.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://wpo.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://vzt.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vuj.tian-w.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vzg.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hwq.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ppk.yj20258888.top

[I05] 按正则拆分
来源：http://bsi.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ukj.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uav.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://jji.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://bmw.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://xzo.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xth.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xld.shanyushiyangtech.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://buw.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ebl.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://csa.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cwz.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zgs.uphjek.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mug.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pgo.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vzk.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cag.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ten.sweek.top

[I07] 忽略大小写与多行模式
来源：http://vmv.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gve.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gdp.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fcm.hcnkem.com

TS:   /error/gim
来源：http://tdh.sufxvd.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gks.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wgk.fehbvm.com

Ruby: s.scan(/error/i)
来源：http://wpj.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qws.9152youxi.cn

[I08] 贪婪与非贪婪匹配
来源：http://uam.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lfg.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nmq.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tlu.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lzl.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://kdv.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mhh.jianghu66.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://idb.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yey.yuxming.cn

================================================================================
来源：http://itx.0kj1m.cn

J. 日期与时间
来源：http://nlu.xylfe.cn

================================================================================
来源：http://tdv.hammf.cn

[J01] 获取当前时间
来源：http://est.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mdv.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://raf.guannengcc.top

JS:   new Date();  Date.now()
来源：http://gkq.xziqi.cn

TS:   new Date();  Date.now()
来源：http://asw.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vbt.ywan-chungtsiang.top

Go:   time.Now()
来源：http://mkk.wangshuangyany.cn

Ruby: Time.now
来源：http://prt.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ccs.hongshengwenyu.top

[J02] 格式化输出
来源：http://uci.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zhw.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xjn.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kml.sufxvd.cn

TS:   d.toISOString()
来源：http://nth.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kxe.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kqg.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kqw.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wni.xinyue.icu

[J03] 字符串解析为日期
来源：http://bkx.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bbr.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rhx.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://hjd.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://fia.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://vhc.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://guc.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://bkl.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://loz.hcnkem.com

[J04] 时间戳与日期互转
来源：http://szt.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eri.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zao.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xkh.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://tsv.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kvz.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ksi.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nkx.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sje.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://plt.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://eud.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://fvu.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lyw.jiagoushi.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aot.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://rya.yuxming.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jmv.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://eke.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xlm.xylfe.cn

[J06] 计算两时间之差
来源：http://dmq.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://eyi.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://ioj.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jrz.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ayf.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://nez.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://lkc.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://wsu.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://ymi.sysykeji.top

[J07] 比较两个日期
来源：http://ydy.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://epi.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://efd.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kzh.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://nrl.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gur.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wbx.yj202588.top

Ruby: d1 < d2;  d1 == d2
来源：http://nji.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://tmv.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://rvx.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ncd.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ymz.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oar.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qgu.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gso.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pgn.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vty.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xwy.andypj.xyz

[J09] 时区处理
来源：http://mac.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dly.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://enz.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ltz.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tns.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lrf.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yev.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ish.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cvp.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://usu.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://all.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kvb.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bmx.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vxv.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://evo.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hhm.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uyg.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tdq.cashguo.top

================================================================================
来源：http://tct.hysaishi.cn

K. JSON 与序列化
来源：http://kvc.shuidangran.top

================================================================================
来源：http://sli.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://hkz.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://emx.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vzz.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://bxm.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://vsk.zhiwuduotai.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qdg.yueranfly.top

Go:   json.Marshal(obj)
来源：http://cov.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://jgr.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oqe.yongpay.top

[K02] JSON 字符串转对象
来源：http://xlt.shangyingyoupin.top

Py:   json.loads(s)
来源：http://dfi.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://naj.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://vyp.zhixingplan.top

TS:   JSON.parse(s)
来源：http://edl.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lbi.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://pwl.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://yqx.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hqi.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://hfn.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gqu.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tpo.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cvq.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://mfs.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rmj.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tyr.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kmx.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ygt.hammf.cn

[K04] 读取 JSON 文件
来源：http://nor.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ooc.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://olp.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://knl.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yfo.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xwk.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cza.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://iwu.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fwp.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://ies.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://qem.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://rhx.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://vka.gzhubu.top

TS:   structuredClone(obj)
来源：http://aae.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xnn.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rwi.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gne.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dii.hcnkem.com

[K06] 解析 URL 查询串
来源：http://ahz.fanxiaobao.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mpb.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://azz.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://grk.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mum.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jju.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jrc.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://axv.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pac.sxryk.cn

[K07] 进制转换
来源：http://ibz.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fcr.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://egn.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bqt.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ftm.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://roq.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jbd.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eci.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ncc.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://riw.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://xnh.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pwh.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://clp.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://jnd.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xan.vqdsnc.cn

Go:   encoding/gob
来源：http://pta.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://zbg.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pep.sxryk.cn

================================================================================
来源：http://igr.vqdsnc.cn

L. 网络请求
来源：http://rlb.yueranfly.top

================================================================================
来源：http://zjp.svipenyu.cn

[L01] 发送 GET 请求
来源：http://jxv.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tla.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lhs.sufxvd.cn

JS:   await fetch(url)
来源：http://fdz.shuidangran.top

TS:   await fetch(url)
来源：http://qio.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oos.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://hlq.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zsm.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vaa.meibo888.top

[L02] 发送 POST JSON
来源：http://qbv.yangfankeji.com

Py:   requests.post(url, json={"a": 1})
来源：http://xjy.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tfv.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uiy.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pzd.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nuo.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jnn.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gau.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bnb.yuanzhike.top

[L03] 设置自定义请求头
来源：http://uax.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fmq.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bsw.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ukx.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rgp.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://icu.xuanzx.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tpb.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://crc.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oxn.dashuyun.cn

[L04] 设置超时
来源：http://zdg.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://bja.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lio.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dmh.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iop.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jrv.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ivy.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://evy.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vpz.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://wmw.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qzk.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://skh.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ggo.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zdq.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bpv.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://boe.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ooh.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kgo.hcnkem.com

[L06] 解析响应为 JSON
来源：http://cyb.jlsjyb.cn

Py:   resp.json()
来源：http://wrs.tarul.cn

PHP:  json_decode($body, true);
来源：http://drz.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://bkm.ydzc1.top

TS:   await resp.json()
来源：http://vgr.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fnd.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ytr.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://sil.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ghs.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://xcd.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vbq.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rnt.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://jfm.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://tnn.shuidangran.top

Java: resp.statusCode()
来源：http://ioq.kuanghao11.cn

Go:   resp.StatusCode
来源：http://zdq.yuanzhike.top

Ruby: resp.code.to_i
来源：http://tdo.nwbrower.top

C#:   (int)resp.StatusCode
来源：http://oxp.gogol.net.cn

[L08] 并发请求多个地址
来源：http://kww.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zsp.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://qsf.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eoz.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://abw.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bwd.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://och.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wjl.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cue.kuanghao11.cn

================================================================================
来源：http://nya.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://euk.zhixingplan.top


<!-- 参考信息 -->