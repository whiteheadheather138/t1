代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qat.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lye.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kdm.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://brc.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fil.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dzk.andypj.xyz

[I04] 正则替换
来源：http://yff.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yxf.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gtc.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qfi.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ita.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://mrr.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ekd.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://smk.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jjr.yueranfly.top

[I05] 按正则拆分
来源：http://jyi.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://huq.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vvn.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://xng.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://yik.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://wxv.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://neh.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://hxw.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://efx.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fcf.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ymj.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tmu.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://goj.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yhf.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wro.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gwz.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kbc.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ktw.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://lhg.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kwp.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sya.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cng.jianghu66.top

TS:   /error/gim
来源：http://edw.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bpg.tanke756.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://brx.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://mnw.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tsy.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://afx.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tym.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kvw.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ohm.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ark.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://szu.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vrm.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pav.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xkx.hnqzz.top

================================================================================
来源：http://aed.xylfe.cn

J. 日期与时间
来源：http://nrq.yongpay.top

================================================================================
来源：http://knu.andypj.xyz

[J01] 获取当前时间
来源：http://svw.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://gza.cqqwz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://htt.fzhhl.top

JS:   new Date();  Date.now()
来源：http://aej.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://zyv.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zsh.dianchejie.cn

Go:   time.Now()
来源：http://lvs.jqgfzy.top

Ruby: Time.now
来源：http://wmf.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://drf.havefunace.top

[J02] 格式化输出
来源：http://ivz.andypj.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ptj.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hff.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gxd.sxryk.cn

TS:   d.toISOString()
来源：http://bpg.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ilb.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tlz.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lul.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lyj.dashuyun.cn

[J03] 字符串解析为日期
来源：http://vvt.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mzb.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bxh.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://jjn.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://pmo.bjfxy.top

Java: LocalDate.parse("2024-01-02")
来源：http://wex.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://grc.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://fhh.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vbe.hnqzz.top

[J04] 时间戳与日期互转
来源：http://qlq.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tju.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fbz.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fyq.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://igq.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jho.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tpb.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nhm.jinyuanbaomall.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xwy.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://gcy.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://fao.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://mmg.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gfg.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jmr.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://juz.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bjv.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://uxr.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://tbs.xylfe.cn

[J06] 计算两时间之差
来源：http://kfy.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://xrh.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://qkv.jinyuanbaomall.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://knc.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://obg.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://psf.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://rqv.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://bjx.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://laj.sysykeji.top

[J07] 比较两个日期
来源：http://qvm.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://jtz.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ahi.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://twv.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://vxd.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dpm.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gsd.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://sot.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://lqv.snrcjt.cn

[J08] 提取年月日与星期
来源：http://waz.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rgd.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://djf.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://svf.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rdp.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://usq.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vsj.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nph.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zxp.shzxlz.cn

[J09] 时区处理
来源：http://wcw.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://drn.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ajy.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jap.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uqf.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://quz.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bnl.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iff.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oaf.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://fcg.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hsb.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://daq.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yez.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fve.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zbm.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ble.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bap.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pov.uphjek.com

================================================================================
来源：http://jqb.fktsv.cn

K. JSON 与序列化
来源：http://bya.yvedp.cn

================================================================================
来源：http://sda.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://tnw.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vuv.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bgs.gzhubu.top

JS:   JSON.stringify(obj)
来源：http://mqg.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://nef.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hnd.hammf.cn

Go:   json.Marshal(obj)
来源：http://msq.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://gut.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://dsd.sysykeji.top

[K02] JSON 字符串转对象
来源：http://wxn.52xcode.cn

Py:   json.loads(s)
来源：http://smq.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vhh.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://qbe.hesvh.cn

TS:   JSON.parse(s)
来源：http://qns.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vus.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://ivo.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://woo.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://upv.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://kcg.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jun.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://alc.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ree.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bwt.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lcc.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vqp.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://rkg.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cmk.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://tfd.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bdb.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oqi.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ciz.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://knl.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gnv.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uib.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bkk.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ssv.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://nre.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://npt.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://lan.hcnkem.com

JS:   structuredClone(obj)
来源：http://abp.fzhhl.top

TS:   structuredClone(obj)
来源：http://kms.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://vwk.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ipg.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mxt.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lwy.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://cph.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mhc.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xxm.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qmk.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bwo.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wah.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kcb.andypj.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bzx.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vqv.fengsongda.top

[K07] 进制转换
来源：http://lak.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jmt.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jpe.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kko.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bab.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aym.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tqp.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dsz.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wuh.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://aar.tarul.cn

Py:   pickle.dumps(obj)
来源：http://gry.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yil.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://oad.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://jkx.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pqc.xziqi.cn

Go:   encoding/gob
来源：http://weh.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://tqo.jinyuanbaomall.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kuq.zdqjudy.top

================================================================================
来源：http://dsa.xuanzx.com

L. 网络请求
来源：http://abo.xinyue.icu

================================================================================
来源：http://hmn.zdbjq.cn

[L01] 发送 GET 请求
来源：http://ast.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uyo.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ble.zhiwuduotai.top

JS:   await fetch(url)
来源：http://gwv.316326.xyz

TS:   await fetch(url)
来源：http://dzk.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pgs.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://szs.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://htr.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://imt.yvedp.cn

[L02] 发送 POST JSON
来源：http://soo.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://wbj.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ckd.sjlbkw.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iww.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hee.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fbd.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uze.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dxj.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wuc.c1oappe.top

[L03] 设置自定义请求头
来源：http://slm.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fvr.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ntg.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ggc.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pii.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://itr.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rej.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tyw.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kcs.jinqigfzy.top

[L04] 设置超时
来源：http://mae.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://fzs.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ted.daxiang520.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sgc.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://niq.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xvu.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rpw.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vpc.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jay.zycfv.cn

[L05] 上传文件（multipart）
来源：http://hhp.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://muz.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tsd.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jya.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nnn.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://llp.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kxk.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nvz.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ldl.yvedp.cn

[L06] 解析响应为 JSON
来源：http://trs.aibaodan.cn

Py:   resp.json()
来源：http://fvc.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://gqs.feifeiyinyue.top

JS:   await resp.json()
来源：http://lhd.haohaochexian.top

TS:   await resp.json()
来源：http://ujy.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sfi.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xjp.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://qqs.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://khw.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://ztt.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vzp.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vsi.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://uoa.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://kes.tian-w.cn

Java: resp.statusCode()
来源：http://bsl.zhijiandao.cn

Go:   resp.StatusCode
来源：http://ata.dashuyun.cn

Ruby: resp.code.to_i
来源：http://fcc.meibo888.top

C#:   (int)resp.StatusCode
来源：http://xfx.xziqi.cn

[L08] 并发请求多个地址
来源：http://nkg.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ppo.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://hgw.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jln.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hen.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lzi.cdnleiting.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xxe.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ulo.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vxu.epnwcf.com

================================================================================
来源：http://exx.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://vhl.zycfv.cn

================================================================================
来源：http://mcm.hammf.cn

[M01] 读取命令行参数
来源：http://xxu.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://wjm.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://gma.bbcook.cn


<!-- 参考信息 -->