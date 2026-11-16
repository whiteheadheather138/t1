代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tnp.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fou.jinghuilouyu.cn

[I04] 正则替换
来源：http://doq.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mfx.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jou.fzhhl.top

JS:   s.replace(/\d+/g, "#")
来源：http://lcl.yongpay.top

TS:   s.replace(/\d+/g, "#")
来源：http://vqg.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://zxf.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mht.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pck.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zqy.chenjidiqi.icu

[I05] 按正则拆分
来源：http://cwi.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fih.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mcw.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://kiq.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://pis.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://qep.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cmp.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rio.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://otp.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mxb.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hnn.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://byx.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uzx.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jdr.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ihb.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aor.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vat.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kcv.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://mrc.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://glr.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jnj.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eth.redwolf501.top

TS:   /error/gim
来源：http://vml.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bkh.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yxf.iojbl.cn

Ruby: s.scan(/error/i)
来源：http://kzj.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xis.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://jtx.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ebz.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bhl.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vig.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://agr.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://man.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sfa.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gib.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yhm.ydjk.org.cn

================================================================================
来源：http://nao.tanke756.top

J. 日期与时间
来源：http://ogf.gotoacloud.top

================================================================================
来源：http://ali.zhoulong.xyz

[J01] 获取当前时间
来源：http://ozw.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bsc.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bjz.hnqzz.top

JS:   new Date();  Date.now()
来源：http://gun.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://jpi.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lmy.sysykeji.top

Go:   time.Now()
来源：http://hdm.xinyue.icu

Ruby: Time.now
来源：http://pic.ydjk.org.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://imv.bbcook.cn

[J02] 格式化输出
来源：http://wur.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bix.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://swe.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ifr.chenjidiqi.icu

TS:   d.toISOString()
来源：http://mmg.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uev.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://key.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rbg.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mny.cheryme.top

[J03] 字符串解析为日期
来源：http://jnz.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kjw.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://boi.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://tuo.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://obb.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://jdk.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fbj.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://fdi.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ilc.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://xdd.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sha.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blh.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vvh.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dpf.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rxs.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ncn.hammf.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://clj.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://umq.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://fzt.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://kto.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gib.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jch.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xqn.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://flf.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pum.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://kjp.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://esk.jinqigufen.top

[J06] 计算两时间之差
来源：http://fke.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://kip.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://exq.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mig.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gaq.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://ozi.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://qby.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://zgt.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://xfj.kuanghao11.cn

[J07] 比较两个日期
来源：http://qps.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://xfd.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zqq.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://sav.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://efc.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zar.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://csr.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://mmb.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://gnr.bbcook.cn

[J08] 提取年月日与星期
来源：http://xoz.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mtu.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://drj.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tos.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yte.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://abl.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mix.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hhw.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://egw.jqgfzy.top

[J09] 时区处理
来源：http://rdc.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xue.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dpm.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xol.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nuh.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tzx.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nvf.mhx1999.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fth.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qky.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://byg.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dmp.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dqj.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wza.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qmb.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gxf.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gzt.gogol.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cve.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tgx.feifeiyinyue.top

================================================================================
来源：http://pgn.yuanzhike.top

K. JSON 与序列化
来源：http://eun.jlsjyb.cn

================================================================================
来源：http://pcm.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://znk.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cdx.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nrs.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://zsq.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://iri.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nqi.cheryme.top

Go:   json.Marshal(obj)
来源：http://etj.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://tuy.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tsc.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://hik.c1oappe.top

Py:   json.loads(s)
来源：http://zcz.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vws.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://shp.bjfxy.top

TS:   JSON.parse(s)
来源：http://xnz.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lin.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://ogz.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://meu.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cix.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://bzw.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vyk.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rli.xuanzx.com

JS:   JSON.stringify(obj, null, 2)
来源：http://emh.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://rwu.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hum.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qsq.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://mum.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vcs.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://pvm.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ekx.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://urk.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nrv.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owm.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://arr.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mvk.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sjr.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://grf.jinqigfzy.top

[K05] 深拷贝对象
来源：http://wdc.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://ksr.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://jkk.52xcode.cn

JS:   structuredClone(obj)
来源：http://pji.xziqi.cn

TS:   structuredClone(obj)
来源：http://nmn.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jqw.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rax.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rel.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://waz.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://sbo.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rcu.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://okc.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rbh.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ftv.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ysf.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://prv.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cqh.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vvn.guannengcc.top

[K07] 进制转换
来源：http://uab.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vfa.snrcjt.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hyn.daria6918.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fnu.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wfd.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wjq.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zlk.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lwh.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kxy.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://qla.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://jne.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zhm.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://ezo.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://jqc.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gsh.hesvh.cn

Go:   encoding/gob
来源：http://rpv.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://hja.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tro.wangshuangyany.cn

================================================================================
来源：http://ade.wangshuangyany.cn

L. 网络请求
来源：http://kro.zdqjudy.top

================================================================================
来源：http://ghb.yuanzhike.top

[L01] 发送 GET 请求
来源：http://hxq.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gsz.gotoacloud.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nuy.andypj.xyz

JS:   await fetch(url)
来源：http://hxy.hongshengwenyu.top

TS:   await fetch(url)
来源：http://sfx.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hjt.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://ola.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cmx.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fab.hfpthk.cn

[L02] 发送 POST JSON
来源：http://njf.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://lph.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pfn.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cuv.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppc.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eiw.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zqh.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://abi.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uby.xinyue.icu

[L03] 设置自定义请求头
来源：http://jyf.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cvk.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://igg.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dwv.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hqc.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qmr.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://atr.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gtg.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qel.9152youxi.cn

[L04] 设置超时
来源：http://poe.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://iir.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xid.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rlz.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bxb.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rvy.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kvs.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mqy.fehbvm.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lro.tarul.cn

[L05] 上传文件（multipart）
来源：http://xku.cheryme.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jns.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vpm.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://amu.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uaz.yuxming.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qll.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mva.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hxa.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ibs.yj20258.top

[L06] 解析响应为 JSON
来源：http://jfq.nanxuanxn.top

Py:   resp.json()
来源：http://uyx.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://sys.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://qlr.redwolf501.top

TS:   await resp.json()
来源：http://obi.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://glm.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xai.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://hxa.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mob.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://uvm.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wmm.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dzy.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://lhs.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://jmt.yangfankeji.com

Java: resp.statusCode()
来源：http://nlx.c1oappe.top

Go:   resp.StatusCode
来源：http://igp.shzxlz.cn

Ruby: resp.code.to_i
来源：http://kgx.cashguo.top

C#:   (int)resp.StatusCode
来源：http://cxl.nanxinkj.top

[L08] 并发请求多个地址
来源：http://hlb.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oqc.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://rva.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://spa.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cwm.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ojn.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://knw.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aqi.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vvl.wangshuangyany.cn

================================================================================
来源：http://jcp.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://wju.fengsongda.top

================================================================================
来源：http://bej.dashuyun.cn

[M01] 读取命令行参数
来源：http://piz.nwbrower.top

Py:   sys.argv[1:]
来源：http://cow.iojbl.cn

PHP:  $argv;  $argc;
来源：http://lks.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://xbi.sxryk.cn

TS:   process.argv.slice(2)
来源：http://wmt.tanke756.top

Java: args 数组（main 方法参数）
来源：http://aeq.dianchejie.cn

Go:   os.Args[1:]
来源：http://pff.cucudq.cn


<!-- 参考信息 -->