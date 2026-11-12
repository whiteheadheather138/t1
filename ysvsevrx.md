代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jyx.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://djv.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://bhd.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://paw.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nrz.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ozb.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ugh.andypj.xyz

[I05] 按正则拆分
来源：http://nyb.kuanghao11.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jrk.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ied.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://rya.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://fru.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://kqd.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rjf.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://amg.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rua.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://irl.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tku.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yes.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ncv.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zzo.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lvp.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ahz.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xyk.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yye.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://dim.c1oappe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wly.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fra.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ihh.bjfxy.top

TS:   /error/gim
来源：http://efi.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hwv.zhaomingkeji.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kzh.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://rio.birdmap.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tiv.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://txe.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fdc.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uex.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kgp.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://atl.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jri.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vdd.tanke756.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pkw.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ofb.xziqi.cn

================================================================================
来源：http://wqz.mhx1999.top

J. 日期与时间
来源：http://rmt.jinqigfzy.top

================================================================================
来源：http://ycp.yj20258.top

[J01] 获取当前时间
来源：http://mqu.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://edp.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jmn.ybcxt.top

JS:   new Date();  Date.now()
来源：http://ujy.mhx1999.top

TS:   new Date();  Date.now()
来源：http://qyn.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aqa.cdnleiting.top

Go:   time.Now()
来源：http://utt.52xcode.cn

Ruby: Time.now
来源：http://bzn.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sqm.zdqjudy.top

[J02] 格式化输出
来源：http://tik.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hot.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bju.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://odt.bbcook.cn

TS:   d.toISOString()
来源：http://rtu.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eci.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vvv.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wmy.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cdd.tarul.cn

[J03] 字符串解析为日期
来源：http://bjj.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://msg.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gux.ivvv.top

JS:   new Date("2024-01-02")
来源：http://lvb.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://meq.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yhy.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gqo.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://xij.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ivy.hnqzz.top

[J04] 时间戳与日期互转
来源：http://duv.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wza.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://khu.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wpl.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ezn.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dkh.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://upw.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cxh.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://krf.cheryme.top

[J05] 时间加减（加 7 天）
来源：http://atp.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://jps.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xpq.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tto.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wji.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://ury.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://awn.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://ifd.smart0.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://sfh.sxryk.cn

[J06] 计算两时间之差
来源：http://squ.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://fpm.zhijiandao.cn

PHP:  $end->diff($start)->days;
来源：http://xyd.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cza.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gzy.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jyx.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://hhs.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://fnj.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://ase.sweek.top

[J07] 比较两个日期
来源：http://vad.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://rcc.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dfm.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://dcb.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://qle.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qbl.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zjs.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://pre.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://ref.cheryme.top

[J08] 提取年月日与星期
来源：http://ikl.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wwz.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oup.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://akb.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yxy.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dvi.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gks.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hsg.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xcg.sufxvd.cn

[J09] 时区处理
来源：http://fmv.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rjm.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mgm.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://czy.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ota.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bvi.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hzn.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://qlk.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xrz.bbcook.cn

[J10] 取今天 / 本月第一天
来源：http://lnm.guowangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vtp.jiagoushi.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dkt.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vgf.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sha.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sfd.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rcw.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oeq.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ofr.yonumen.top

================================================================================
来源：http://tbl.chenlongwang.top

K. JSON 与序列化
来源：http://drs.fehbvm.com

================================================================================
来源：http://rmh.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://yqw.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mzn.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wqa.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://fbt.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://dyh.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nbm.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://yxq.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://mxl.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nfu.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://ufb.iojbl.cn

Py:   json.loads(s)
来源：http://tfl.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vwz.zycfv.cn

JS:   JSON.parse(s)
来源：http://wla.gotoacloud.top

TS:   JSON.parse(s)
来源：http://djk.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xth.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://btb.iojbl.cn

Ruby: JSON.parse(s)
来源：http://klj.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vdh.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://hap.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mmk.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hqx.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lny.cashguo.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sqi.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yrq.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iii.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://acr.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tan.c1oappe.top

[K04] 读取 JSON 文件
来源：http://dyo.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://czk.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cvh.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://msg.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pvu.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lqt.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oqs.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ztr.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://new.cqqwz.cn

[K05] 深拷贝对象
来源：http://akf.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://fci.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://wnz.9152youxi.cn

JS:   structuredClone(obj)
来源：http://qar.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://gxw.bbcook.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gty.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tcf.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mzc.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zmp.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://lyf.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jjy.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cxt.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wou.yuanzhike.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xlv.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://agp.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rtr.xinyue.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nxp.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fgo.yonumen.top

[K07] 进制转换
来源：http://tbr.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qgf.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hrf.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ebl.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wou.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://noh.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ktg.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cwn.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://obw.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://fiw.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://niw.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://olg.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://tjp.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://kqe.sufxvd.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ckh.zhoulong.xyz

Go:   encoding/gob
来源：http://jkb.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://jfs.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jfa.yongpay.top

================================================================================
来源：http://miv.jqgufenzy.top

L. 网络请求
来源：http://vye.daria6918.cn

================================================================================
来源：http://xpx.hcnkem.com

[L01] 发送 GET 请求
来源：http://rfq.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rru.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dcp.ivvv.top

JS:   await fetch(url)
来源：http://vga.9152youxi.cn

TS:   await fetch(url)
来源：http://edq.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nru.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://oln.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rvl.sjlbkw.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qkl.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://ilv.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vbe.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wlu.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ylt.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fyd.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://upk.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ubk.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lgd.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://biw.tanke756.top

[L03] 设置自定义请求头
来源：http://vdr.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://avj.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fmy.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bjt.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hcb.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cuz.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://crd.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zew.jinyuanbaomall.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nzg.fktsv.cn

[L04] 设置超时
来源：http://ypc.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://oxe.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iwa.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ahw.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lvz.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zkf.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fjl.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oag.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wvg.sxryk.cn

[L05] 上传文件（multipart）
来源：http://htz.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hxg.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sjg.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fya.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lea.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fqt.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xoc.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ccj.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gvx.52xcode.cn

[L06] 解析响应为 JSON
来源：http://wyd.zhaomingkeji.xyz

Py:   resp.json()
来源：http://twj.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://snq.pycfn.com

JS:   await resp.json()
来源：http://foz.yj20258.top

TS:   await resp.json()
来源：http://xxq.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://awx.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jkc.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://mxi.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ztf.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://izw.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zbt.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cfm.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://wuc.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://lpd.cdnleiting.top

Java: resp.statusCode()
来源：http://ihy.gotoacloud.top

Go:   resp.StatusCode
来源：http://lwt.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://xyc.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://trn.yj20258.top

[L08] 并发请求多个地址
来源：http://efp.yj202588.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cmy.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://rht.jinghuilouyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sso.yj20258.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tjg.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://juv.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qwc.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hea.vehdjk.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ibn.shuidangran.top

================================================================================
来源：http://wjv.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://hcl.jyoumei.cn

================================================================================
来源：http://duy.yvedp.cn

[M01] 读取命令行参数
来源：http://msk.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://ebg.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://wxz.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://gnx.tarul.cn

TS:   process.argv.slice(2)
来源：http://mpn.yueranfly.top

Java: args 数组（main 方法参数）
来源：http://iys.jyoumei.cn

Go:   os.Args[1:]
来源：http://qdn.jqgufenzy.top

Ruby: ARGV
来源：http://dis.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://fsp.xziqi.cn

[M02] 读取环境变量
来源：http://bbw.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://ugp.jqgufenzy.top


<!-- 参考信息 -->