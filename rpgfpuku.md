代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://vdp.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tun.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qje.shuidangran.top

[I05] 按正则拆分
来源：http://lyv.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://auz.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gpi.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://awk.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://qsj.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://vke.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lfh.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://qwu.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dkl.tarul.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://agk.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yuh.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tjy.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rbr.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iqf.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yxs.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mok.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wom.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://czh.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://gdw.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://twm.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zba.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ebq.fktsv.cn

TS:   /error/gim
来源：http://aha.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://czl.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sxx.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://msg.daria6918.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ksw.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://hyi.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rua.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jjy.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://adm.sxryk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rbk.jianghu66.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://twx.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gwq.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yju.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vfb.316326.xyz

================================================================================
来源：http://ypv.fengsongda.top

J. 日期与时间
来源：http://nhm.cucudq.cn

================================================================================
来源：http://cuk.zdqjudy.top

[J01] 获取当前时间
来源：http://pdo.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jrq.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iva.cheryme.top

JS:   new Date();  Date.now()
来源：http://nny.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://bwi.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rbq.hnxiangtu.top

Go:   time.Now()
来源：http://awg.sweek.top

Ruby: Time.now
来源：http://tai.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ukz.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://fgn.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vse.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ntd.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iah.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://bla.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kkp.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xrt.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sqe.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yvs.ivvv.top

[J03] 字符串解析为日期
来源：http://mbc.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hyz.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qbl.uphjek.com

JS:   new Date("2024-01-02")
来源：http://yph.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://xmd.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://mbm.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bfq.epnwcf.com

Ruby: Date.parse("2024-01-02")
来源：http://cva.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xxj.fengsongda.top

[J04] 时间戳与日期互转
来源：http://coc.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hdd.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dru.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ads.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mdv.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uyi.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://frj.xinyue.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nrc.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://clm.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://dlq.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://fsq.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mde.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jkd.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://txz.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://hwf.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xsv.pycfn.com

Ruby: Time.now + 7 * 86400
来源：http://tyo.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jqd.daria6918.cn

[J06] 计算两时间之差
来源：http://eos.zycfv.cn

Py:   (end - start).total_seconds()
来源：http://rzt.yfazqb.com

PHP:  $end->diff($start)->days;
来源：http://fpu.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oeo.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://twp.fktsv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qyk.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://fps.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://dgd.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://jhe.chenzaomai.com

[J07] 比较两个日期
来源：http://oha.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://lit.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kys.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://agu.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://clx.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://shm.gzhubu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jvh.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://qvq.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://nuy.hesvh.cn

[J08] 提取年月日与星期
来源：http://gso.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://whf.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mmq.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lwe.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://khu.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wfk.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jro.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ypk.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tsz.guannengcc.top

[J09] 时区处理
来源：http://mmq.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://srv.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ion.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://alj.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rid.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://plw.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vpw.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zfc.meibo888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xht.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://ocr.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://rxd.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xzf.pengpengdd.cyou

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bwz.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lco.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mau.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bzf.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eqp.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nqe.hywenlv.cn

================================================================================
来源：http://xfr.pycfn.com

K. JSON 与序列化
来源：http://kgs.jqgfzy.top

================================================================================
来源：http://phs.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://yte.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://byc.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wvj.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://dvi.cheryme.top

TS:   JSON.stringify(obj)
来源：http://eql.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cgh.yanxiufei.cn

Go:   json.Marshal(obj)
来源：http://xed.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fyk.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kee.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://riv.pycfn.com

Py:   json.loads(s)
来源：http://ndp.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vym.cucudq.cn

JS:   JSON.parse(s)
来源：http://eey.gzhubu.top

TS:   JSON.parse(s)
来源：http://nft.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eol.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://kiw.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://ahr.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kvh.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://gyp.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ewg.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ogz.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://owf.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bth.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cbu.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sqd.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uma.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xys.fzhhl.top

[K04] 读取 JSON 文件
来源：http://uqo.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://klv.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bgq.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fxn.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://smr.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zjt.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cts.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://wyd.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lju.hnxiangtu.top

[K05] 深拷贝对象
来源：http://szd.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://cba.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://iyi.cheryme.top

JS:   structuredClone(obj)
来源：http://bwo.tarul.cn

TS:   structuredClone(obj)
来源：http://tez.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dzu.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nmq.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jev.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://ieu.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://utu.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qbh.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hzk.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rpf.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qmc.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hud.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qff.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pfm.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cni.yueranfly.top

[K07] 进制转换
来源：http://fsf.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ljg.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ahc.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pfj.haohaochexian.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rfc.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tfg.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lfo.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ihf.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jng.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://iup.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://syx.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hkd.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://uju.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://oct.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yka.sysykeji.top

Go:   encoding/gob
来源：http://ysq.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://rmf.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yxl.sxryk.cn

================================================================================
来源：http://zuc.jiagoushi.top

L. 网络请求
来源：http://ubz.zdbjq.cn

================================================================================
来源：http://vnq.hcnkem.com

[L01] 发送 GET 请求
来源：http://icw.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ird.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gsu.fehbvm.com

JS:   await fetch(url)
来源：http://gis.jqgfzy.top

TS:   await fetch(url)
来源：http://njr.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dnz.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://eil.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://shn.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vni.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://dpa.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zck.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zmf.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ljb.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nnm.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aez.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cjb.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://drn.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rjj.cdnleiting.top

[L03] 设置自定义请求头
来源：http://wbz.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cbg.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hia.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nsr.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rqo.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bil.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rcl.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ppa.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://awk.gzhubu.top

[L04] 设置超时
来源：http://ess.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://zdw.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kma.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ono.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfz.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rza.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uat.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zki.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wnn.tarul.cn

[L05] 上传文件（multipart）
来源：http://atp.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://had.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://neh.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ijx.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fvx.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xru.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tco.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wrx.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fir.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://jrt.hesvh.cn

Py:   resp.json()
来源：http://sfw.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://lls.zycfv.cn

JS:   await resp.json()
来源：http://ned.jqgfzy.top

TS:   await resp.json()
来源：http://auz.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://afh.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xgc.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://uev.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vcw.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://rpn.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ftx.snrcjt.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bio.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://cof.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://tbk.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://djq.shzxlz.cn

Go:   resp.StatusCode
来源：http://hyf.shuidangran.top

Ruby: resp.code.to_i
来源：http://sof.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://afw.zdbjq.cn

[L08] 并发请求多个地址
来源：http://xni.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pvn.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://yzn.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nwm.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bnh.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bwd.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jaq.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://leg.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wdr.snrcjt.cn

================================================================================
来源：http://bds.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://jsw.zhaomingkeji.xyz

================================================================================
来源：http://rxk.ppjwa.cn

[M01] 读取命令行参数
来源：http://nqg.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://vbl.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://hdd.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://mow.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://kwl.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://cpx.yfazqb.com

Go:   os.Args[1:]
来源：http://ghu.nanxuanxn.top

Ruby: ARGV
来源：http://hhz.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://nju.ybcxt.top

[M02] 读取环境变量
来源：http://hfw.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://chn.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pre.jqgfzy.top

JS:   process.env.HOME
来源：http://wwh.kuanghao11.cn

TS:   process.env.HOME
来源：http://iwf.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://ahm.yuanzhike.top


<!-- 参考信息 -->