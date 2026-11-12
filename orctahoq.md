代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kla.epnwcf.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qyc.tianlin.xyz

[I04] 正则替换
来源：http://bvb.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nbz.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iqp.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://bgr.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://uqy.bjfxy.top

Java: s.replaceAll("\\d+", "#")
来源：http://jmr.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uax.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://zje.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://any.pycfn.com

[I05] 按正则拆分
来源：http://xxq.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lcu.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jsb.yvedp.cn

JS:   s.split(/\s*,\s*/)
来源：http://aei.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://nbu.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://swu.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nwo.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://olm.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qkp.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://weo.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ucx.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ezn.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dyo.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://raq.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dkv.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ltu.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://npn.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ycz.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://ocs.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lhh.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uen.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://arp.pycfn.com

TS:   /error/gim
来源：http://ueg.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xmc.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gyf.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://eoa.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://krp.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://pct.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jfx.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rih.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tre.jianghu66.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zcw.nanxinkj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kya.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xrq.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tky.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://acf.vehdjk.com

================================================================================
来源：http://yne.hywenlv.cn

J. 日期与时间
来源：http://rel.ivvv.top

================================================================================
来源：http://kwl.ppjwa.cn

[J01] 获取当前时间
来源：http://euo.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bom.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jle.yj20258888.top

JS:   new Date();  Date.now()
来源：http://rsg.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://zsi.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jhs.xinyue.icu

Go:   time.Now()
来源：http://diq.chenjidiqi.icu

Ruby: Time.now
来源：http://bhk.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fgf.316326.xyz

[J02] 格式化输出
来源：http://tgx.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eps.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gax.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fzz.zdqjudy.top

TS:   d.toISOString()
来源：http://nii.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://poo.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xbc.andypj.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xdl.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pxx.chenlongwang.top

[J03] 字符串解析为日期
来源：http://fel.shangyingyoupin.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pry.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://msr.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://jxl.yongpay.top

TS:   new Date("2024-01-02")
来源：http://fhq.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://yci.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wci.hywenlv.cn

Ruby: Date.parse("2024-01-02")
来源：http://qfu.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jmg.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://nls.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://olq.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ojl.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zas.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bys.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ttz.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pvs.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rue.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fco.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://aeq.yj20258.top

Py:   now + timedelta(days=7)
来源：http://elo.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://snv.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ooh.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yyk.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://ukh.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bjt.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://jha.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gdh.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://rnn.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://xlh.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://fjm.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gpm.52xcode.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oom.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://adf.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://rru.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://oru.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://sqi.c1oappe.top

[J07] 比较两个日期
来源：http://yui.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://hwk.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oep.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://meo.zdbjq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oyr.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://igc.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nev.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://ckm.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://iyx.9152youxi.cn

[J08] 提取年月日与星期
来源：http://quo.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://szk.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://she.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ngr.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qad.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lmx.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fpo.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tci.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hkk.hnqzz.top

[J09] 时区处理
来源：http://pna.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oqv.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ixc.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pww.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kqi.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jeh.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lgl.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://exo.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nzq.0kj1m.cn

[J10] 取今天 / 本月第一天
来源：http://dyw.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://sjx.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qlz.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dcm.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fmy.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://icu.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kxq.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xle.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://twp.yj20258888.top

================================================================================
来源：http://hsl.jinqigufen.top

K. JSON 与序列化
来源：http://kli.zdqjudy.top

================================================================================
来源：http://coc.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://jbv.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jdc.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cge.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://txk.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://ozw.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ahc.mhx1999.top

Go:   json.Marshal(obj)
来源：http://bau.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://wnb.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://nyw.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://acj.chenlongwang.top

Py:   json.loads(s)
来源：http://ywj.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jsw.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://kly.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://uqo.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ewv.316326.xyz

Go:   json.Unmarshal(data, &v)
来源：http://vcb.xinyue.icu

Ruby: JSON.parse(s)
来源：http://lya.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sbb.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://rsp.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kkb.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ziz.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yua.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mpb.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lhf.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dfj.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://zdm.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dcc.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://wtq.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://myy.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://alq.jinqigufen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ulg.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mbg.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://usy.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pga.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://sdo.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aoq.yuanzhike.top

[K05] 深拷贝对象
来源：http://wpe.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://pnx.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://rbf.havefunace.top

JS:   structuredClone(obj)
来源：http://knn.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://jhr.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://flu.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ybo.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zsv.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://blp.daxiang520.top

[K06] 解析 URL 查询串
来源：http://thj.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oxf.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://riu.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxc.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sqc.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qye.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ndp.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hwf.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://twp.bjfxy.top

[K07] 进制转换
来源：http://oly.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kha.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pzc.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wwd.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nhq.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hbp.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ztf.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mex.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cep.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://vzs.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://kcj.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tyg.dashuyun.cn

JS:   v8.serialize(obj)        // Node
来源：http://bcq.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://nnr.yongpay.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xyz.sweek.top

Go:   encoding/gob
来源：http://pqo.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://acc.xingfuxueyuan.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gjv.hysaishi.cn

================================================================================
来源：http://jyr.havefunace.top

L. 网络请求
来源：http://wxg.pengpengdd.cyou

================================================================================
来源：http://wgg.yueranfly.top

[L01] 发送 GET 请求
来源：http://qtg.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gmo.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rpx.sufxvd.cn

JS:   await fetch(url)
来源：http://pus.zhijiandao.cn

TS:   await fetch(url)
来源：http://tcg.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pjb.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://nek.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://fql.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vfx.cheryme.top

[L02] 发送 POST JSON
来源：http://nkc.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://cgf.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rfq.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hmf.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kao.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qdm.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fdp.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bxu.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ynh.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://owy.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ltj.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wpl.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lnm.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sxd.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ovb.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kjh.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dok.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lkf.fzhhl.top

[L04] 设置超时
来源：http://ulb.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://smi.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qfr.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xhz.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://klg.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jtg.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fuz.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qvf.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ymf.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://iby.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nzg.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wyn.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hhs.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://akh.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mxl.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kri.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uai.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://smq.tarul.cn

[L06] 解析响应为 JSON
来源：http://ynd.zhiwuduotai.top

Py:   resp.json()
来源：http://bot.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://lnz.jinghuilouyu.cn

JS:   await resp.json()
来源：http://xdp.xziqi.cn

TS:   await resp.json()
来源：http://puf.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gzd.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lek.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://pql.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qos.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://tjc.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fqm.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://obs.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://afo.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://hvq.gotoacloud.top

Java: resp.statusCode()
来源：http://wlj.mhx1999.top

Go:   resp.StatusCode
来源：http://grf.bbcook.cn

Ruby: resp.code.to_i
来源：http://rvc.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://ldp.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://ppt.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ukx.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://ufj.xingfuxueyuan.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gws.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wah.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lnz.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://llv.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qkm.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hux.yanxiufei.cn

================================================================================
来源：http://rck.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://sso.yvedp.cn

================================================================================
来源：http://lpr.fengsongda.top

[M01] 读取命令行参数
来源：http://nir.cqqwz.cn

Py:   sys.argv[1:]
来源：http://pah.pycfn.com

PHP:  $argv;  $argc;
来源：http://wgx.havefunace.top

JS:   process.argv.slice(2)
来源：http://bcg.xinyue.icu

TS:   process.argv.slice(2)
来源：http://xlf.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://vhe.zhoulong.xyz

Go:   os.Args[1:]
来源：http://dnb.aizwys.cn


<!-- 参考信息 -->