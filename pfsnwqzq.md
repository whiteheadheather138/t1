代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qbc.yj20258888.top

[I03] 提取捕获分组
来源：http://gfa.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vga.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yeb.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aao.daria6918.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://njj.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://obu.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ckq.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ejk.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oep.birdmap.top

[I04] 正则替换
来源：http://owh.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nzl.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fhu.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://rig.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://puw.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cji.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ryx.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uwy.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gpe.feifeiyinyue.top

[I05] 按正则拆分
来源：http://hum.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rqa.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pal.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://bdh.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://hhg.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://mzk.cqqwz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pdm.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://ren.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://slj.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wnu.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tss.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qxg.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hao.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wnj.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cdd.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wmd.cheryme.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gav.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sqn.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://yrr.nanxuanxn.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yvm.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vut.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yuc.meibo888.top

TS:   /error/gim
来源：http://gzv.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ywt.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yan.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://dma.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pbb.shanyushiyangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://yor.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bpx.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://czs.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ekr.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kuw.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qgk.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cqf.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pqb.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://apo.ctjpmb.com

================================================================================
来源：http://rzj.yj20258888.top

J. 日期与时间
来源：http://oro.uphjek.com

================================================================================
来源：http://cwt.sysykeji.top

[J01] 获取当前时间
来源：http://kmj.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://url.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zzs.ivvv.top

JS:   new Date();  Date.now()
来源：http://tuj.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://jhd.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ope.snrcjt.cn

Go:   time.Now()
来源：http://obk.snrcjt.cn

Ruby: Time.now
来源：http://hwx.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://avl.gogol.net.cn

[J02] 格式化输出
来源：http://oan.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yvm.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qjq.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xax.bbcook.cn

TS:   d.toISOString()
来源：http://wov.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dah.mhx1999.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cui.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kin.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lhz.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://gtf.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tix.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hws.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://yml.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://djv.tianlin.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://cjo.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zut.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://riy.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bzy.vehdjk.com

[J04] 时间戳与日期互转
来源：http://vdv.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fef.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mnv.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kcg.hcnkem.com

TS:   Math.floor(Date.now() / 1000)
来源：http://men.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://asa.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wbe.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nbj.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fsx.bbcook.cn

[J05] 时间加减（加 7 天）
来源：http://try.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://cvx.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://gyz.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dzt.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pfu.zycfv.cn

Java: LocalDate.now().plusDays(7)
来源：http://ajf.daxiang520.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jeb.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://yog.hongshengwenyu.top

C#:   DateTime.Now.AddDays(7)
来源：http://ram.yanxiufei.cn

[J06] 计算两时间之差
来源：http://qky.yongpay.top

Py:   (end - start).total_seconds()
来源：http://cft.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://ikn.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mly.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gpf.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://bzz.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://usi.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://mao.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://rga.havefunace.top

[J07] 比较两个日期
来源：http://sgs.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://tsd.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zhs.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://tmk.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://srh.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hcj.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://umo.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vca.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://vel.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://vcn.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://emh.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zgr.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pkr.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://juu.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cux.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oay.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rmk.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bhs.zycfv.cn

[J09] 时区处理
来源：http://irx.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://woy.gotoacloud.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hil.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sbp.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://siv.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xzc.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rxg.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ged.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hlf.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://ysi.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tsj.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bwm.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dah.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ocr.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pfm.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ohy.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dkc.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gse.redwolf501.top

================================================================================
来源：http://ucl.redwolf501.top

K. JSON 与序列化
来源：http://ksl.hysaishi.cn

================================================================================
来源：http://gtn.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://kge.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zte.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fmz.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://rie.yonumen.top

TS:   JSON.stringify(obj)
来源：http://dyh.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://szk.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://ljt.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iak.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hmu.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://mnb.epnwcf.com

Py:   json.loads(s)
来源：http://eir.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uep.yj202588.top

JS:   JSON.parse(s)
来源：http://biz.xuanzx.com

TS:   JSON.parse(s)
来源：http://zfz.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mle.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://kxi.xuanzx.com

Ruby: JSON.parse(s)
来源：http://abd.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vhw.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://hwo.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dpp.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zjt.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hyo.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ack.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fpp.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jwh.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://hgx.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jgn.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://nne.yuxming.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hwu.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qxc.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rpc.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ala.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oam.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zbt.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sny.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mnn.sysykeji.top

[K05] 深拷贝对象
来源：http://nfv.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://icu.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://hwa.jianghu66.top

JS:   structuredClone(obj)
来源：http://zbc.yvedp.cn

TS:   structuredClone(obj)
来源：http://nld.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://qdc.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ykc.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vou.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kmg.yj202588.top

[K06] 解析 URL 查询串
来源：http://xdt.hesvh.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xjm.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mxw.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yho.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tqf.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ecn.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tni.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vew.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://snr.epnwcf.com

[K07] 进制转换
来源：http://gsx.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pln.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mqk.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lzf.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xyd.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://spq.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://edd.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://miz.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://twg.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://cvq.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://roy.yangfankeji.com

PHP:  serialize($obj);  unserialize($s);
来源：http://waw.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://ebk.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://vvr.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yjg.tian-w.cn

Go:   encoding/gob
来源：http://glt.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://fot.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bvs.xuetiantiany.cn

================================================================================
来源：http://tyj.gaohongyu789.top

L. 网络请求
来源：http://bce.xziqi.cn

================================================================================
来源：http://agd.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://rab.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ddv.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fvg.andypj.xyz

JS:   await fetch(url)
来源：http://ajf.zdqjudy.top

TS:   await fetch(url)
来源：http://zcf.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bhf.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://ipw.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://acw.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lna.mhx1999.top

[L02] 发送 POST JSON
来源：http://eaz.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wdy.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jvh.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fhe.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fsb.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://arr.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fcp.jianghu66.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sqe.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cfq.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://esr.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dvj.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mxn.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hvg.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqf.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://prj.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sgm.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qfi.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sli.sufxvd.cn

[L04] 设置超时
来源：http://gsp.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://oqa.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://foe.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://owt.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hnh.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yuv.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pcc.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ibd.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aej.tanke756.top

[L05] 上传文件（multipart）
来源：http://wxk.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pyw.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ivd.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kgf.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rrb.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xcn.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pft.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pmn.ehwqpu.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tsq.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://qmc.xinyue.icu

Py:   resp.json()
来源：http://lqu.cucudq.cn

PHP:  json_decode($body, true);
来源：http://qow.fzhhl.top

JS:   await resp.json()
来源：http://ndt.guannengcc.top

TS:   await resp.json()
来源：http://bjg.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qdh.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mdg.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://mgk.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kax.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://hsn.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nck.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bdu.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://beo.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://hht.jinqigfzy.top

Java: resp.statusCode()
来源：http://ecq.ivvv.top

Go:   resp.StatusCode
来源：http://qdr.redwolf501.top

Ruby: resp.code.to_i
来源：http://imd.yj20258.top

C#:   (int)resp.StatusCode
来源：http://txu.xinyue.icu

[L08] 并发请求多个地址
来源：http://tmq.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kpu.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://kkt.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://omd.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckd.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xxf.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wwp.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wrq.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ojb.jiagoushi.top

================================================================================
来源：http://ckh.sweek.top

M. 命令行 / 进程 / 环境
来源：http://ibb.tarul.cn


<!-- 参考信息 -->