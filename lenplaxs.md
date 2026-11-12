代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zrh.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ijd.yj20258888.top

[I04] 正则替换
来源：http://hqy.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fjg.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://khv.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ana.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://zxk.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://qty.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://kdj.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wrq.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://asd.kuanghao11.cn

[I05] 按正则拆分
来源：http://syo.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mtm.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iix.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://rvf.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://snl.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://hht.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://she.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rze.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qhy.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mvg.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eld.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://koi.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uxk.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://otf.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ruy.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cpn.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rwg.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sir.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://ycu.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lpq.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pjx.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fsy.feifeiyinyue.top

TS:   /error/gim
来源：http://iid.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jhh.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rzm.chenlongwang.top

Ruby: s.scan(/error/i)
来源：http://qsm.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aox.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://loz.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bze.jqgfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eez.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kpx.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://apl.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://fro.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mnk.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fnn.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vtd.yvedp.cn

================================================================================
来源：http://hmv.jiagoushi.top

J. 日期与时间
来源：http://wdx.nanxinkj.top

================================================================================
来源：http://nbc.jinqigufen.top

[J01] 获取当前时间
来源：http://ftb.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cue.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fwr.tarul.cn

JS:   new Date();  Date.now()
来源：http://ssw.kuanghao11.cn

TS:   new Date();  Date.now()
来源：http://dyt.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zdt.gaohongyu789.top

Go:   time.Now()
来源：http://zci.wangshuangyany.cn

Ruby: Time.now
来源：http://smi.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bvw.316326.xyz

[J02] 格式化输出
来源：http://twq.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ytx.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sah.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sxt.tian-w.cn

TS:   d.toISOString()
来源：http://lyd.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hky.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vbf.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ktq.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hmm.0kj1m.cn

[J03] 字符串解析为日期
来源：http://txj.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://htg.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zlj.birdmap.top

JS:   new Date("2024-01-02")
来源：http://noc.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://gcr.pengpengdd.cyou

Java: LocalDate.parse("2024-01-02")
来源：http://gur.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ztm.jlsjyb.cn

Ruby: Date.parse("2024-01-02")
来源：http://gpc.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bpg.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://yvw.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kel.ivvv.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qxz.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ujk.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://khj.dianchejie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ypg.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://scf.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ljk.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hki.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://qwv.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://csp.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ito.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kxm.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dre.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://hir.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rnn.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://oom.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://tga.ppjwa.cn

[J06] 计算两时间之差
来源：http://czw.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://lgb.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://qlh.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://krq.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bxh.jlsjyb.cn

Java: Duration.between(start, end).toSeconds()
来源：http://psr.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://ygt.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://gch.sysykeji.top

C#:   (end - start).TotalSeconds
来源：http://jtt.shuidangran.top

[J07] 比较两个日期
来源：http://sdi.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://toz.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gxx.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://ppc.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://tbx.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wgv.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wcs.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://dne.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://qiw.haohaochexian.top

[J08] 提取年月日与星期
来源：http://smp.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ykw.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nai.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qna.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rlg.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://att.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pyu.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fcp.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vfu.fehbvm.com

[J09] 时区处理
来源：http://esj.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bwi.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://meu.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jib.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yht.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://elr.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lza.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rfe.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wcj.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://asg.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://ahj.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fsx.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://adg.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yjf.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cny.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://waq.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vmi.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nyg.cucudq.cn

================================================================================
来源：http://ffi.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://jud.cashguo.top

================================================================================
来源：http://sxb.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://bri.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yuh.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kwo.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://cgr.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://kxx.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://utj.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://pkw.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://iur.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wah.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://gpe.yfazqb.com

Py:   json.loads(s)
来源：http://vrv.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eqm.yuxming.cn

JS:   JSON.parse(s)
来源：http://rux.shzxlz.cn

TS:   JSON.parse(s)
来源：http://utq.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ham.hcnkem.com

Go:   json.Unmarshal(data, &v)
来源：http://dwk.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://mvj.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gma.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://mjv.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lco.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ayc.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://vsn.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lgo.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vne.xuetiantiany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gyg.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://rjk.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ifl.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://gja.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fco.yfazqb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fxa.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qbi.ydjk.org.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kbf.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hju.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bex.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://omx.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ino.fzhhl.top

[K05] 深拷贝对象
来源：http://kqk.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://oig.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://zby.kuanghao11.cn

JS:   structuredClone(obj)
来源：http://hph.cdnleiting.top

TS:   structuredClone(obj)
来源：http://xwn.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://axi.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zlf.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ctz.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ely.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://jwo.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ccm.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mgd.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gme.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://paw.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yxd.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wzz.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ftb.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kko.zdqjudy.top

[K07] 进制转换
来源：http://mpn.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jvn.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://okq.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ere.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ajt.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jdi.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wig.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yvq.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nhw.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://pkw.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://ovn.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qit.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://khu.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://pst.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zjl.52xcode.cn

Go:   encoding/gob
来源：http://agc.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://ckd.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ubo.nanxinkj.top

================================================================================
来源：http://ibc.xziqi.cn

L. 网络请求
来源：http://zgz.shuidangran.top

================================================================================
来源：http://lck.sweek.top

[L01] 发送 GET 请求
来源：http://zzo.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mdz.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://riw.jinqigfzy.top

JS:   await fetch(url)
来源：http://ssv.hongshengwenyu.top

TS:   await fetch(url)
来源：http://ewc.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zjg.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://uqc.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://qla.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kdc.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://svg.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://cbv.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yxo.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sbd.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fyh.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wwk.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qoq.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wal.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mae.jqgfzy.top

[L03] 设置自定义请求头
来源：http://neb.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://smp.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mrd.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yyo.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qhu.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://znc.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mng.zhixingplan.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nao.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yjj.epnwcf.com

[L04] 设置超时
来源：http://jvs.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://oho.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dld.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kzy.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tdq.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tdo.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ury.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ugi.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://clx.wangshuangyany.cn

[L05] 上传文件（multipart）
来源：http://cos.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xqu.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kst.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rkw.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bsm.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://isc.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lhh.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jno.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ncv.ydzc1.top

[L06] 解析响应为 JSON
来源：http://lae.xuanzx.com

Py:   resp.json()
来源：http://ykh.nwbrower.top

PHP:  json_decode($body, true);
来源：http://mcn.gotoacloud.top

JS:   await resp.json()
来源：http://dbl.fehbvm.com

TS:   await resp.json()
来源：http://mdl.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lwe.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sci.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://nxx.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://igd.fehbvm.com

[L07] 处理 HTTP 状态码
来源：http://twg.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tgm.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dtw.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://ehj.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://eyn.hcnkem.com

Java: resp.statusCode()
来源：http://yww.yj20258888.top

Go:   resp.StatusCode
来源：http://gyj.havefunace.top

Ruby: resp.code.to_i
来源：http://wid.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://wnb.sweek.top

[L08] 并发请求多个地址
来源：http://lhc.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cpb.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://rtw.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://smz.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cfv.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zgi.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nxb.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mid.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gfe.0kj1m.cn

================================================================================
来源：http://ech.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://ihi.tanke756.top

================================================================================
来源：http://sdr.jyoumei.cn

[M01] 读取命令行参数
来源：http://qro.daria6918.cn

Py:   sys.argv[1:]
来源：http://btg.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://ehw.hesvh.cn

JS:   process.argv.slice(2)
来源：http://pdx.sxryk.cn

TS:   process.argv.slice(2)
来源：http://bhw.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://odr.havefunace.top

Go:   os.Args[1:]
来源：http://tvf.jlsjyb.cn


<!-- 参考信息 -->