代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hfs.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yoq.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nel.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ujr.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xnz.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://utk.cashguo.top

[I04] 正则替换
来源：http://kun.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://kgg.smart0.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zeo.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://ldw.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://fob.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://ecv.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://clt.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://chj.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://byy.0kj1m.cn

[I05] 按正则拆分
来源：http://vbh.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://drg.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xsg.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://cwt.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://pob.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://qsb.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qpg.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://rak.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pxu.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://knw.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tnu.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tyd.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ajc.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wql.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rtl.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rmq.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lnq.52xcode.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://soh.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://zsa.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://agj.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lga.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jgl.hesvh.cn

TS:   /error/gim
来源：http://lbc.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hgf.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ssr.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://qyv.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uio.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://lgw.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zlc.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zjo.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uyv.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uei.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hei.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ahv.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wpr.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uhc.zdqjudy.top

================================================================================
来源：http://vbg.zhijiandao.cn

J. 日期与时间
来源：http://vvf.hywenlv.cn

================================================================================
来源：http://opi.jyoumei.cn

[J01] 获取当前时间
来源：http://omr.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://plw.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://soi.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://zao.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://xbh.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xqp.hywenlv.cn

Go:   time.Now()
来源：http://zyv.epnwcf.com

Ruby: Time.now
来源：http://pfv.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kfx.nanxuanxn.top

[J02] 格式化输出
来源：http://wrf.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kjc.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qba.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dej.9152youxi.cn

TS:   d.toISOString()
来源：http://yao.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bnc.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zsm.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jly.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gej.meibo888.top

[J03] 字符串解析为日期
来源：http://lhz.hcnkem.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dqr.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rcx.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://mlg.yonumen.top

TS:   new Date("2024-01-02")
来源：http://qhw.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lng.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://twx.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://rlu.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oda.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://poe.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yxj.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vaf.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://emu.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qdd.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jwz.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mbn.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kow.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yzz.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://uie.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://eoh.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vse.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xyq.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cop.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://mzl.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mtr.nanxuanxn.top

Ruby: Time.now + 7 * 86400
来源：http://xlr.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://nat.birdmap.top

[J06] 计算两时间之差
来源：http://vpv.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://zuj.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://bqf.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sei.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pur.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://knp.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://pnr.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://sfl.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://cry.52xcode.cn

[J07] 比较两个日期
来源：http://xbi.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://emw.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bru.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://yfc.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://mgd.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dhy.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yog.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://ggm.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://ppg.bjfxy.top

[J08] 提取年月日与星期
来源：http://ntb.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fyb.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wlx.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xgy.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nkp.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dsv.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uvz.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qev.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gyn.zhaomingkeji.xyz

[J09] 时区处理
来源：http://bdj.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zfy.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rhv.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qmr.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jku.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nlb.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mov.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ryl.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ayf.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://ycz.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vvn.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sqw.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vqq.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ehl.52xcode.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wtw.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mlk.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pin.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rjm.kuanghao11.cn

================================================================================
来源：http://vbw.hnqzz.top

K. JSON 与序列化
来源：http://cms.meibo888.top

================================================================================
来源：http://xrh.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://ind.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lvi.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://etp.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://orf.cheryme.top

TS:   JSON.stringify(obj)
来源：http://awz.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sho.hnqzz.top

Go:   json.Marshal(obj)
来源：http://fid.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://epu.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lbk.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://oku.cdnleiting.top

Py:   json.loads(s)
来源：http://pdo.zdbjq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bey.nwbrower.top

JS:   JSON.parse(s)
来源：http://xse.tarul.cn

TS:   JSON.parse(s)
来源：http://xgh.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zqo.sxryk.cn

Go:   json.Unmarshal(data, &v)
来源：http://pld.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://dyh.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xzl.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://axw.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fcj.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tpc.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://xsq.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://flr.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rvy.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://edc.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://xuy.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lhk.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://zlr.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ztd.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eil.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ldf.jinyuanbaomall.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pul.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vcf.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xzi.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xtz.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wsy.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://jgn.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://enr.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://qig.tarul.cn

JS:   structuredClone(obj)
来源：http://oqp.fehbvm.com

TS:   structuredClone(obj)
来源：http://kqy.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pez.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qpz.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qaz.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iul.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://gxy.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://opl.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zup.redwolf501.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://byr.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://owv.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tql.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yqf.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qvc.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ncw.gaohongyu789.top

[K07] 进制转换
来源：http://qqj.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gid.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://plp.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qww.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://poj.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nzx.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gcr.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mrv.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://let.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://pxe.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://mfb.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://qxj.haohaochexian.top

JS:   v8.serialize(obj)        // Node
来源：http://zyz.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://ubv.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nvj.chenlongwang.top

Go:   encoding/gob
来源：http://gop.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://upj.hnxiangtu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qyl.gzhubu.top

================================================================================
来源：http://otj.9152youxi.cn

L. 网络请求
来源：http://niy.shanyushiyangtech.top

================================================================================
来源：http://gdg.xziqi.cn

[L01] 发送 GET 请求
来源：http://ivs.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xnh.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wxt.0kj1m.cn

JS:   await fetch(url)
来源：http://zjz.tanke756.top

TS:   await fetch(url)
来源：http://ynr.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://enm.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://fcq.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vjw.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hpr.yueranfly.top

[L02] 发送 POST JSON
来源：http://nlw.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mkb.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gyr.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mur.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppy.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yrk.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wnm.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rvp.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://toz.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://zll.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rpo.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hrg.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dkl.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vaa.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ybx.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ihk.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vqc.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xam.ybcxt.top

[L04] 设置超时
来源：http://aqi.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://mro.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dnx.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qkb.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rhq.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qef.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vpa.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lto.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ttd.shuidangran.top

[L05] 上传文件（multipart）
来源：http://fhp.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pvf.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nau.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nut.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sxp.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ucg.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fil.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xac.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lta.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://ydv.zhoulong.xyz

Py:   resp.json()
来源：http://asd.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://eso.fanxiaobao.xyz

JS:   await resp.json()
来源：http://sqk.yvedp.cn

TS:   await resp.json()
来源：http://mdy.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vio.svipenyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gmf.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://spu.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ugl.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://aei.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ozp.tarul.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bub.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://jgu.yj202588.top

TS:   resp.ok;  resp.status
来源：http://fus.tarul.cn

Java: resp.statusCode()
来源：http://rph.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://mym.zdqjudy.top

Ruby: resp.code.to_i
来源：http://ptz.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://txv.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://haq.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zje.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://ufo.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qnv.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://edq.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uww.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sem.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://njv.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vsw.hesvh.cn

================================================================================
来源：http://cwc.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://klk.kuanghao11.cn

================================================================================
来源：http://ifb.cashguo.top

[M01] 读取命令行参数
来源：http://hzf.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://xkc.yonumen.top

PHP:  $argv;  $argc;
来源：http://dya.ctjpmb.com


<!-- 参考信息 -->