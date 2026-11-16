代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lkf.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wzd.ydzc1.top

[I04] 正则替换
来源：http://jqv.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://iov.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://znb.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://sku.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://pnm.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://tyf.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://azc.xuetiantiany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dou.andypj.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zmb.dashuyun.cn

[I05] 按正则拆分
来源：http://rkf.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://qhx.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hos.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://ifj.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://apv.yueranfly.top

Java: s.split("\\s*,\\s*")
来源：http://tsb.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vce.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rrp.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mqe.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rlx.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://egc.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ade.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kqh.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://prs.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pbv.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://otp.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://thu.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hdk.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://sml.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://suq.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://omi.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yiz.nanxuanxn.top

TS:   /error/gim
来源：http://ftr.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pcm.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tel.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://wzk.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ctt.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://evk.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cxl.guowangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://otx.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://obj.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ylx.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://rqe.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vid.fktsv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tfg.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kfe.hnxiangtu.top

================================================================================
来源：http://kfw.chenjidiqi.icu

J. 日期与时间
来源：http://bbr.zhaomingkeji.xyz

================================================================================
来源：http://lob.gogol.net.cn

[J01] 获取当前时间
来源：http://lng.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ynb.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://agh.tian-w.cn

JS:   new Date();  Date.now()
来源：http://awf.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://rgo.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zik.jlsjyb.cn

Go:   time.Now()
来源：http://dnf.hesvh.cn

Ruby: Time.now
来源：http://fuu.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://laf.yfazqb.com

[J02] 格式化输出
来源：http://kom.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nyz.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mlu.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wbu.shuidangran.top

TS:   d.toISOString()
来源：http://cjo.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://khc.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ecp.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wxh.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eka.yangfankeji.com

[J03] 字符串解析为日期
来源：http://lij.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://buo.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wxq.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://wul.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://ife.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://rpl.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hcs.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://pav.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://csi.ivvv.top

[J04] 时间戳与日期互转
来源：http://fto.snrcjt.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://shh.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jhv.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://poe.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ohs.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dcv.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vpk.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ghv.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zxw.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://phw.yj202588.top

Py:   now + timedelta(days=7)
来源：http://vpx.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mpl.havefunace.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xbb.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pah.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://mcf.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://evh.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://nyg.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://jer.vqdsnc.cn

[J06] 计算两时间之差
来源：http://sdr.ivvv.top

Py:   (end - start).total_seconds()
来源：http://fde.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://rdz.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wlt.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://chy.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://fns.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://flt.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://csu.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://yve.ydjk.org.cn

[J07] 比较两个日期
来源：http://hjo.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://nsn.andypj.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ehh.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://xfd.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://cdi.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jqc.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rei.havefunace.top

Ruby: d1 < d2;  d1 == d2
来源：http://tjf.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://kkt.yuxming.cn

[J08] 提取年月日与星期
来源：http://nyc.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dad.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gfu.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ghg.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zzj.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bbl.sxryk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gqo.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tdk.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mrr.chenjidiqi.icu

[J09] 时区处理
来源：http://rel.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dos.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dnk.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://age.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://niw.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qqk.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jgc.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gju.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vja.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://dgk.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cwq.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xfy.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tia.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mkh.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vgt.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nfr.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fof.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ura.fanxiaobao.xyz

================================================================================
来源：http://xyp.sweek.top

K. JSON 与序列化
来源：http://xbj.vqdsnc.cn

================================================================================
来源：http://bll.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://oss.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eyb.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dxx.sweek.top

JS:   JSON.stringify(obj)
来源：http://xar.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://jig.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fzh.zhengqikj.top

Go:   json.Marshal(obj)
来源：http://lzr.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://bkj.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://zns.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://fge.ybcxt.top

Py:   json.loads(s)
来源：http://qnv.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://edp.jqgfzy.top

JS:   JSON.parse(s)
来源：http://ksp.cashguo.top

TS:   JSON.parse(s)
来源：http://ahf.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ohe.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://ejx.guannengcc.top

Ruby: JSON.parse(s)
来源：http://qah.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uyf.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://dun.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vzb.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gtt.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mkc.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://opq.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nfu.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rob.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://zpf.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ibt.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://ukv.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nzk.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wdq.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fjv.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ktb.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vud.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iry.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qll.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xgm.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://dyw.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://qap.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://qal.shanyushiyangkeji.top

JS:   structuredClone(obj)
来源：http://jly.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://ldu.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://amy.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fsa.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://agk.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hth.ivvv.top

[K06] 解析 URL 查询串
来源：http://kaz.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zob.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wpd.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wux.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ykx.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://snx.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://zfi.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wwo.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zpu.jyoumei.cn

[K07] 进制转换
来源：http://qoy.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fsx.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ito.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qqm.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xeb.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tkx.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hsp.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zkl.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mgu.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://tbx.yvedp.cn

Py:   pickle.dumps(obj)
来源：http://boy.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://klr.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://jwz.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://unu.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aci.mhx1999.top

Go:   encoding/gob
来源：http://avg.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://reb.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lzs.xinyue.icu

================================================================================
来源：http://iix.jinghuilouyu.cn

L. 网络请求
来源：http://pdg.ybcxt.top

================================================================================
来源：http://pwe.cheryme.top

[L01] 发送 GET 请求
来源：http://kva.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cke.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zhx.316326.xyz

JS:   await fetch(url)
来源：http://gep.zhoulong.xyz

TS:   await fetch(url)
来源：http://uhw.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zef.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://ezq.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oyz.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uly.andypj.xyz

[L02] 发送 POST JSON
来源：http://pne.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://yoc.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://afo.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gmv.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cfu.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qmi.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uvn.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gau.pycfn.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mgw.yuanzhike.top

[L03] 设置自定义请求头
来源：http://ees.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oea.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vql.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ovf.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ksl.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yxm.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wcy.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://erd.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ubd.chenzaomai.com

[L04] 设置超时
来源：http://vle.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://wxr.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zrl.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ttz.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fmu.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jqr.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pbv.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vyr.yj20258888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yso.yueranfly.top

[L05] 上传文件（multipart）
来源：http://lrt.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hgq.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wdi.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rmm.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eqg.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jom.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xcn.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wad.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lln.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://jwb.hfpthk.cn

Py:   resp.json()
来源：http://wdk.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://kgc.shanyushiyangtech.top

JS:   await resp.json()
来源：http://dje.hnqzz.top

TS:   await resp.json()
来源：http://pfx.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://olg.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lrw.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://nta.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://obc.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://bbs.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://laa.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://myl.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://lhz.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://nse.shzxlz.cn

Java: resp.statusCode()
来源：http://fwn.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://lzx.fktsv.cn

Ruby: resp.code.to_i
来源：http://jzz.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://fwu.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://xkp.quarkkingdee.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eau.sweek.top

PHP:  curl_multi_init() 系列
来源：http://pfp.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://exv.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oue.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uwo.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zkj.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hqx.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ybh.xuanzx.com

================================================================================
来源：http://nxj.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://dzl.xinyue.icu

================================================================================
来源：http://mzz.nanxuanxn.top

[M01] 读取命令行参数
来源：http://jsz.hammf.cn

Py:   sys.argv[1:]
来源：http://oor.yvedp.cn

PHP:  $argv;  $argc;
来源：http://yut.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://uwy.yongpay.top

TS:   process.argv.slice(2)
来源：http://lpg.yj202588.top

Java: args 数组（main 方法参数）
来源：http://fdj.jianghu66.top

Go:   os.Args[1:]
来源：http://snn.jyoumei.cn


<!-- 参考信息 -->