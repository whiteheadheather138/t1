代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rmp.ehwqpu.com

[I03] 提取捕获分组
来源：http://mzi.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cxv.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qzg.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://chl.yonumen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vds.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yym.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gno.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lxo.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lvd.hywenlv.cn

[I04] 正则替换
来源：http://ims.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://oqb.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xfc.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vke.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://wkg.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://fff.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eko.yangfankeji.com

Ruby: s.gsub(/\d+/, "#")
来源：http://mjp.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dub.jianghu66.top

[I05] 按正则拆分
来源：http://qqz.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://bzi.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ssz.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://svr.yj20258.top

TS:   s.split(/\s*,\s*/)
来源：http://zgv.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://hqq.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://alx.cqqwz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gmf.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tre.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://luw.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ikm.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nft.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pdd.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ibg.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vqq.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ojg.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://reg.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rwm.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://rnc.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ips.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://exw.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qcr.kuanghao11.cn

TS:   /error/gim
来源：http://ykn.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cpa.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wsa.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://cbl.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ogm.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://nbz.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cav.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pdp.birdmap.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kqe.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lol.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bsx.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cfj.meibo888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ckv.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dhc.nanxinkj.top

================================================================================
来源：http://aos.hongshengwenyu.top

J. 日期与时间
来源：http://fnu.sxryk.cn

================================================================================
来源：http://zuz.zhijiandao.cn

[J01] 获取当前时间
来源：http://wtf.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jvu.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rrm.bbcook.cn

JS:   new Date();  Date.now()
来源：http://rtr.hesvh.cn

TS:   new Date();  Date.now()
来源：http://ihd.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lcp.hesvh.cn

Go:   time.Now()
来源：http://wpq.wangdashe.top

Ruby: Time.now
来源：http://tez.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dzv.yj20258.top

[J02] 格式化输出
来源：http://jay.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bbq.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lup.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iec.cdnleiting.top

TS:   d.toISOString()
来源：http://mgc.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://clt.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://duf.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wud.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://stp.cucudq.cn

[J03] 字符串解析为日期
来源：http://ptk.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wcd.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qzz.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://lhr.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://tqk.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://vdq.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gnx.xylfe.cn

Ruby: Date.parse("2024-01-02")
来源：http://ymj.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lxr.fzhhl.top

[J04] 时间戳与日期互转
来源：http://ayd.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pna.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ucy.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://asv.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://com.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vsf.chenjidiqi.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://acb.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xek.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bmw.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://kez.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://mta.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://csu.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zpo.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aue.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://osp.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://svy.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://rwc.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://xdf.shzxlz.cn

[J06] 计算两时间之差
来源：http://naa.0kj1m.cn

Py:   (end - start).total_seconds()
来源：http://ojl.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://qix.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xkv.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cyg.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://xpx.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://ufa.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://lbi.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://aqq.ehwqpu.com

[J07] 比较两个日期
来源：http://pbl.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://xcr.bjfxy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eiu.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tlw.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://flu.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vnv.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wty.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qnx.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://qxl.yangfankeji.com

[J08] 提取年月日与星期
来源：http://sqz.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://okr.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zsm.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yep.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oan.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sma.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wim.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://psq.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://smc.hnqzz.top

[J09] 时区处理
来源：http://woq.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gfx.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kot.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wbg.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fjh.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tuv.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iuh.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nfp.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kcf.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://bjv.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ukz.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jye.xuanzx.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vqt.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hhr.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nje.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kzm.andypj.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pck.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wnh.jiagoushi.top

================================================================================
来源：http://vbz.jqgufenzy.top

K. JSON 与序列化
来源：http://wek.0kj1m.cn

================================================================================
来源：http://mtb.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://ybl.fktsv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gdp.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vvr.tarul.cn

JS:   JSON.stringify(obj)
来源：http://usr.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://sam.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cwh.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://xip.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://kfx.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ekq.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://uqk.xuanzx.com

Py:   json.loads(s)
来源：http://iof.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cxe.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://ydq.aizwys.cn

TS:   JSON.parse(s)
来源：http://mkt.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pje.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://hir.daria6918.cn

Ruby: JSON.parse(s)
来源：http://chi.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xit.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://bcx.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://frd.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qay.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dtv.guowangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lhj.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://beh.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dbh.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gzi.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kbo.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://zgg.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jln.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ljf.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pap.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dbf.snrcjt.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yhz.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qwd.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kcw.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oeh.guannengcc.top

[K05] 深拷贝对象
来源：http://pde.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://txj.bbcook.cn

PHP:  unserialize(serialize($obj));
来源：http://sub.ehwqpu.com

JS:   structuredClone(obj)
来源：http://rmp.yj202588.top

TS:   structuredClone(obj)
来源：http://uud.zycfv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vbw.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://alp.fanxiaobao.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://feg.cqqwz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://amr.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://zkq.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://atu.hysaishi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fwh.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bwu.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://isw.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pxp.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tjk.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://has.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xxw.gogol.net.cn

[K07] 进制转换
来源：http://jfu.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kdv.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ght.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wrl.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://exf.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xhe.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ylb.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fvy.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ody.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://zuy.meibo888.top

Py:   pickle.dumps(obj)
来源：http://qvq.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xyd.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://ryy.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://fcv.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lmn.fengsongda.top

Go:   encoding/gob
来源：http://csd.zhaomingkeji.xyz

Ruby: Marshal.dump(obj)
来源：http://ymb.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ycn.yuxming.cn

================================================================================
来源：http://avm.mhx1999.top

L. 网络请求
来源：http://fwr.vehdjk.com

================================================================================
来源：http://iix.ywan-chungtsiang.top

[L01] 发送 GET 请求
来源：http://yae.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hbx.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qne.chenlongwang.top

JS:   await fetch(url)
来源：http://qyl.sxryk.cn

TS:   await fetch(url)
来源：http://urb.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ksv.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://bpd.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kun.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://toc.316326.xyz

[L02] 发送 POST JSON
来源：http://dug.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rao.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vxk.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mda.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fsa.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fzm.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rgt.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kiv.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://svd.sweek.top

[L03] 设置自定义请求头
来源：http://kxw.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nhv.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cjb.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mzx.redwolf501.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://isp.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://puu.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wmo.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jcw.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lpm.hcnkem.com

[L04] 设置超时
来源：http://fxf.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://plh.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ecw.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kpr.tanke756.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vtn.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kwg.zdbjq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bja.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://erq.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hxf.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://rib.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bna.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qfs.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jfe.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jjl.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qic.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dnn.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hkg.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tyc.redwolf501.top

[L06] 解析响应为 JSON
来源：http://tbk.guannengcc.top

Py:   resp.json()
来源：http://gkg.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://fgj.jinqigufen.top

JS:   await resp.json()
来源：http://lju.zycfv.cn

TS:   await resp.json()
来源：http://ojt.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jqw.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ztr.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://knv.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dig.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://xgc.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lzr.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aok.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://cly.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://unl.andypj.xyz

Java: resp.statusCode()
来源：http://mwe.0kj1m.cn

Go:   resp.StatusCode
来源：http://ovh.ybcxt.top

Ruby: resp.code.to_i
来源：http://ctq.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://xzz.epnwcf.com

[L08] 并发请求多个地址
来源：http://dgy.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nrc.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://kca.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://arq.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://llc.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pcl.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xsw.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gbb.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hit.guannengcc.top

================================================================================
来源：http://fwi.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://wwb.jqgufenzy.top


<!-- 参考信息 -->