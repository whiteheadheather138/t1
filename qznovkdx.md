代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://tze.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aik.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://qom.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://mgm.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://lda.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gdh.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vpm.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eon.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://djn.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xwn.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nrg.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hmd.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ngz.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baw.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://keg.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ilk.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jdi.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://bod.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://snb.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://twe.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ivt.9152youxi.cn

TS:   /error/gim
来源：http://pvj.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://joq.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pik.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://ush.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bfn.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://lgj.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tgn.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qpo.haohaochexian.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://usj.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fyv.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zao.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lhj.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://viw.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://urt.hammf.cn

================================================================================
来源：http://leu.fengsongda.top

J. 日期与时间
来源：http://vwv.fehbvm.com

================================================================================
来源：http://pqj.andypj.xyz

[J01] 获取当前时间
来源：http://hse.c1oappe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qic.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ibi.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://tsg.cashguo.top

TS:   new Date();  Date.now()
来源：http://icm.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tlw.dashuyun.cn

Go:   time.Now()
来源：http://oez.yuxming.cn

Ruby: Time.now
来源：http://zos.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vny.aibaodan.cn

[J02] 格式化输出
来源：http://axe.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mot.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gpd.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pcm.jqgufenzy.top

TS:   d.toISOString()
来源：http://tzg.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wwk.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bcl.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nzb.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zcc.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://elf.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oik.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qvt.316326.xyz

JS:   new Date("2024-01-02")
来源：http://wix.sweek.top

TS:   new Date("2024-01-02")
来源：http://amx.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://vof.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iba.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://xib.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uvt.c1oappe.top

[J04] 时间戳与日期互转
来源：http://cva.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ffd.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://brh.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nqs.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://phe.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wtp.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://trk.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lxc.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fzh.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://fnq.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://hom.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sdk.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zqe.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vnn.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://syl.ctjpmb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xfy.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://vnw.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bkm.uphjek.com

[J06] 计算两时间之差
来源：http://utn.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://fmh.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://lom.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pwa.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xax.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://llu.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://gkp.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://wba.hnxiangtu.top

C#:   (end - start).TotalSeconds
来源：http://gij.guannengcc.top

[J07] 比较两个日期
来源：http://opt.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://fen.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pza.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://dkj.chenlongwang.top

TS:   d1.getTime() < d2.getTime()
来源：http://dre.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://shv.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zpp.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://tll.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://bfz.fzhhl.top

[J08] 提取年月日与星期
来源：http://rwa.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://guq.hysaishi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lgy.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bwe.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rho.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kfh.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oxj.sufxvd.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vyn.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://riz.tianlin.xyz

[J09] 时区处理
来源：http://wal.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sch.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mhw.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jyw.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kpr.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nvm.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://edb.yuxming.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://otx.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eig.yj20258888.top

[J10] 取今天 / 本月第一天
来源：http://iey.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://tvf.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zwv.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hcv.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bxb.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xzt.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cpc.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://toy.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jtc.zhaomingkeji.xyz

================================================================================
来源：http://hqj.zhixingplan.top

K. JSON 与序列化
来源：http://srx.sxryk.cn

================================================================================
来源：http://wjp.sweek.top

[K01] 对象转 JSON 字符串
来源：http://ncx.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qhl.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dux.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://yuv.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://tyj.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eic.ivvv.top

Go:   json.Marshal(obj)
来源：http://ipz.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mjr.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hie.xziqi.cn

[K02] JSON 字符串转对象
来源：http://wwp.shzxlz.cn

Py:   json.loads(s)
来源：http://qty.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://smj.gogol.net.cn

JS:   JSON.parse(s)
来源：http://mbc.52xcode.cn

TS:   JSON.parse(s)
来源：http://hto.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fdr.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://zmf.xziqi.cn

Ruby: JSON.parse(s)
来源：http://vhl.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ngj.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://uek.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://agu.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cin.fktsv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nxg.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dbg.0kj1m.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jct.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mxy.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://sbb.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oxu.yongpay.top

[K04] 读取 JSON 文件
来源：http://fdr.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jdw.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vam.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xhl.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kmp.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pkt.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wkn.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yrq.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sci.hesvh.cn

[K05] 深拷贝对象
来源：http://yqw.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://goa.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://ovh.jiagoushi.top

JS:   structuredClone(obj)
来源：http://lcq.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://vzy.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uum.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uij.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vma.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nyy.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://myi.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://der.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wfr.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wfk.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pay.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ubj.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://bbq.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jou.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pyc.hfpthk.cn

[K07] 进制转换
来源：http://rya.yuxming.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://arf.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ery.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wpt.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pye.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wpg.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dri.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://asn.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://smx.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://hcp.tianlin.xyz

Py:   pickle.dumps(obj)
来源：http://scm.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://enz.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://ssz.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://agp.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://usy.jinqigufen.top

Go:   encoding/gob
来源：http://jla.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://tuf.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dwf.zhaomingkeji.xyz

================================================================================
来源：http://qmd.smart0.xyz

L. 网络请求
来源：http://rtb.ivvv.top

================================================================================
来源：http://eye.vehdjk.com

[L01] 发送 GET 请求
来源：http://icx.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://paq.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ucf.hywenlv.cn

JS:   await fetch(url)
来源：http://tjb.gogol.net.cn

TS:   await fetch(url)
来源：http://dvy.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gyl.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://tbu.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://htw.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lsf.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://xrq.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://par.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ocd.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://epg.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hgn.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://csf.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kmk.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fzq.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zba.gotoacloud.top

[L03] 设置自定义请求头
来源：http://flb.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mzs.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nlv.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eua.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://voj.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rlh.andypj.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://att.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://duw.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cyu.daria6918.cn

[L04] 设置超时
来源：http://wjc.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://amg.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lbd.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ujk.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tjk.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qcw.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://var.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kgm.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vsl.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://tvk.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wwx.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://woy.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://njg.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://czt.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wdn.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ctq.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yys.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yhm.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://hql.yj20258888.top

Py:   resp.json()
来源：http://wwm.ydzc1.top

PHP:  json_decode($body, true);
来源：http://edv.jiagoushi.top

JS:   await resp.json()
来源：http://fng.daxiang520.top

TS:   await resp.json()
来源：http://mop.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jrd.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cks.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://rwi.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oeb.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://ywi.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kvu.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zgm.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://oqb.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://mvm.hnxiangtu.top

Java: resp.statusCode()
来源：http://qem.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://kim.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://del.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://xxh.fzhhl.top

[L08] 并发请求多个地址
来源：http://bth.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lia.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://auy.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ein.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wym.sysykeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://awu.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mht.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cip.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wbh.fehbvm.com

================================================================================
来源：http://etz.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://qis.jqgfzy.top

================================================================================
来源：http://dqk.xziqi.cn

[M01] 读取命令行参数
来源：http://jni.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://oxv.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://bcq.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://euj.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://uyb.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://pcv.jqgufenzy.top

Go:   os.Args[1:]
来源：http://vmh.yangfankeji.com

Ruby: ARGV
来源：http://pin.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://mgj.9152youxi.cn

[M02] 读取环境变量
来源：http://jjo.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://mth.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jxn.xuetiantiany.cn

JS:   process.env.HOME
来源：http://cks.zhiwuduotai.top

TS:   process.env.HOME
来源：http://pcc.tarul.cn

Java: System.getenv("HOME")
来源：http://eoh.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ocn.epnwcf.com

Ruby: ENV["HOME"]
来源：http://arj.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fol.vehdjk.com

[M03] 执行外部命令
来源：http://xof.shzxlz.cn


<!-- 参考信息 -->