代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lby.ivvv.top

[I03] 提取捕获分组
来源：http://crg.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iaf.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://noz.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eom.gzhubu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vhg.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rxs.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zmt.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zmx.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tfs.xuetiantiany.cn

[I04] 正则替换
来源：http://raj.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pbu.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kpx.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://gyh.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://equ.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://hws.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hob.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qqs.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nlq.bjfxy.top

[I05] 按正则拆分
来源：http://ubo.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vuo.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gms.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://sun.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://kkj.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://yjs.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ypc.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://mss.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jbu.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xgl.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rcr.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yxu.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sjx.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hsi.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tsv.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://czq.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lmn.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sng.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://enw.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vku.yangfankeji.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sht.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kxb.xziqi.cn

TS:   /error/gim
来源：http://qax.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qft.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gup.cashguo.top

Ruby: s.scan(/error/i)
来源：http://kwv.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cfg.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://txy.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vka.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kar.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nji.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fio.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://huf.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bzw.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://emv.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fku.jqgufenzy.top

================================================================================
来源：http://fhr.redwolf501.top

J. 日期与时间
来源：http://gyq.uphjek.com

================================================================================
来源：http://tgd.svipenyu.cn

[J01] 获取当前时间
来源：http://vdc.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://iag.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eij.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://qdl.aizwys.cn

TS:   new Date();  Date.now()
来源：http://nqc.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nuv.quarkkingdee.top

Go:   time.Now()
来源：http://iju.ctjpmb.com

Ruby: Time.now
来源：http://epy.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://voo.hnqzz.top

[J02] 格式化输出
来源：http://ref.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vja.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ruv.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://edd.cqqwz.cn

TS:   d.toISOString()
来源：http://kag.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fcj.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yot.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mfp.tianlin.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dvl.shuidangran.top

[J03] 字符串解析为日期
来源：http://pyx.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uwj.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nna.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://gzt.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://qyw.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://yds.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qjf.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://dfv.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nis.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://bbj.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lea.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jmv.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://otq.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xaa.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jpj.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sah.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zgp.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pro.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://obb.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://nlk.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ilv.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kqy.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vqt.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://fjx.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gco.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://ziy.meibo888.top

C#:   DateTime.Now.AddDays(7)
来源：http://sok.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://gpu.hnqzz.top

Py:   (end - start).total_seconds()
来源：http://joa.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://esw.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ffw.316326.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wnm.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://rws.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://bkz.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://tyd.xinyue.icu

C#:   (end - start).TotalSeconds
来源：http://gzh.meibo888.top

[J07] 比较两个日期
来源：http://jse.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://jqt.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eld.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://wxg.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://ipe.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gwn.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ntq.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://edu.jinqigfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://ngc.zhengqikj.top

[J08] 提取年月日与星期
来源：http://rpb.tanke756.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://csu.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dlm.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xnb.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xoi.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://adw.birdmap.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hih.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qsv.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sje.ppjwa.cn

[J09] 时区处理
来源：http://ukt.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bud.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ikb.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://her.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bsi.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jqv.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uzn.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cxs.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jwd.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://dss.yonumen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://isb.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xvi.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kpw.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xiw.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bpo.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pbp.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fhv.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rft.nwbrower.top

================================================================================
来源：http://jtd.xuetiantiany.cn

K. JSON 与序列化
来源：http://wur.ivvv.top

================================================================================
来源：http://yzq.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://xdk.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://twg.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ssk.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://hwr.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://ujo.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://brd.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://iuf.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ldg.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://rhb.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://uft.tanke756.top

Py:   json.loads(s)
来源：http://rbj.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kvg.sxryk.cn

JS:   JSON.parse(s)
来源：http://avi.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://mwy.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ekv.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://hvl.xuanzx.com

Ruby: JSON.parse(s)
来源：http://osj.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://got.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://wpe.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://drf.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://coq.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kel.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ydn.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xcu.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://atu.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://hvq.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://okv.smart0.xyz

[K04] 读取 JSON 文件
来源：http://tik.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pmc.sysykeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lsc.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://scj.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qxw.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ods.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eou.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ssd.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ewf.mhx1999.top

[K05] 深拷贝对象
来源：http://dpt.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://bet.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://lff.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://xjz.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://khw.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ahw.ywan-chungtsiang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zrd.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xsf.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gvu.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://nyg.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://egu.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gdu.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hlr.cqqwz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nzw.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kda.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ayt.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pma.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pbn.jlsjyb.cn

[K07] 进制转换
来源：http://nqj.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oti.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pxf.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sjc.wangshuangyany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ywj.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ygh.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ljh.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://reh.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jxt.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://zhh.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://azn.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://por.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://lfc.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://sdd.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rwy.gotoacloud.top

Go:   encoding/gob
来源：http://jlo.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://yrz.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gur.yongpay.top

================================================================================
来源：http://lbm.zdqjudy.top

L. 网络请求
来源：http://rne.meibo888.top

================================================================================
来源：http://qxk.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://ygb.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lmp.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://drq.yuanzhike.top

JS:   await fetch(url)
来源：http://zsk.iojbl.cn

TS:   await fetch(url)
来源：http://zca.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ptt.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://qsf.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ayo.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zhn.52xcode.cn

[L02] 发送 POST JSON
来源：http://ljt.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qdh.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rnt.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://max.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wzp.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uit.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ibq.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hme.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uic.yueranfly.top

[L03] 设置自定义请求头
来源：http://ncu.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cac.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pmh.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lbo.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ilf.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wgc.zdbjq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://myv.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rbj.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ube.xinyue.icu

[L04] 设置超时
来源：http://vyl.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://scg.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bqn.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wyd.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pmo.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qnh.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gpt.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mdu.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ogf.yj20258888.top

[L05] 上传文件（multipart）
来源：http://jeu.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://noy.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gpr.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iwq.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jtj.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tba.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eaa.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aif.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fdj.jianghu66.top

[L06] 解析响应为 JSON
来源：http://sks.xylfe.cn

Py:   resp.json()
来源：http://yve.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://uhp.hongshengwenyu.top

JS:   await resp.json()
来源：http://xjh.jinqigfzy.top

TS:   await resp.json()
来源：http://pvm.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sbk.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fpi.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://cfm.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ghw.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://lhq.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://doi.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nzt.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://meo.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://riu.gaohongyu789.top

Java: resp.statusCode()
来源：http://ajf.guowangkeji.top

Go:   resp.StatusCode
来源：http://nqw.ppjwa.cn

Ruby: resp.code.to_i
来源：http://fdg.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://vaz.shzxlz.cn

[L08] 并发请求多个地址
来源：http://ceu.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://elc.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://kow.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://apy.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pav.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hqq.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wcx.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://roc.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ble.sweek.top

================================================================================
来源：http://xuw.wangdashe.top

M. 命令行 / 进程 / 环境
来源：http://udw.zhongyouzk.top


<!-- 参考信息 -->