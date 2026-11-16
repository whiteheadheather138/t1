代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cew.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qnj.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xzi.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hjj.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nlx.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rsu.jinqigfzy.top

[I04] 正则替换
来源：http://pog.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jlv.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lfk.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://aeg.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rme.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://fww.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xkb.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://krw.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xwo.jianghu66.top

[I05] 按正则拆分
来源：http://geb.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://fca.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iff.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://puw.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://qca.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://mzf.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qkh.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://etw.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vyj.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tlc.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rvz.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gmk.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jqh.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://foa.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ulx.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sib.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xyt.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bbp.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://yqk.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tjw.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qog.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lsk.cdnleiting.top

TS:   /error/gim
来源：http://xrc.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qms.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gmh.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://dff.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ekn.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://rrm.jlsjyb.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bpf.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eew.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oem.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cps.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jci.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://onj.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ble.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qkd.zdbjq.cn

================================================================================
来源：http://tuv.fehbvm.com

J. 日期与时间
来源：http://vqp.zycfv.cn

================================================================================
来源：http://gas.sufxvd.cn

[J01] 获取当前时间
来源：http://jrt.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mga.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qyo.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://ghs.yj202588.top

TS:   new Date();  Date.now()
来源：http://ozg.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yki.xuanzx.com

Go:   time.Now()
来源：http://njn.bbcook.cn

Ruby: Time.now
来源：http://jvc.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fgh.dashuyun.cn

[J02] 格式化输出
来源：http://vhe.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sbl.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yay.pycfn.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rlr.gogol.net.cn

TS:   d.toISOString()
来源：http://wlq.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://feu.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://etb.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://chj.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pyg.tian-w.cn

[J03] 字符串解析为日期
来源：http://rqr.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rdn.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bgs.yonumen.top

JS:   new Date("2024-01-02")
来源：http://oye.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://jmy.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://tyj.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ees.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://hyr.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gcj.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://tdh.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lyd.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ort.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tyc.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://fjs.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://srz.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jyh.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rsm.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://axo.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://wja.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://hrx.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://skm.ybcxt.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lcz.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ifp.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://vly.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xre.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://kgz.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://fvj.shuidangran.top

[J06] 计算两时间之差
来源：http://xzv.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://don.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://puq.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mte.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://duo.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ptn.daxiang520.top

Go:   end.Sub(start).Hours()
来源：http://fpe.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://mun.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://ilw.pycfn.com

[J07] 比较两个日期
来源：http://qnx.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://slr.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xmr.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://uvl.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lkw.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://byg.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mot.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pkf.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://xca.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://gqg.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jcw.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://anc.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jyb.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hiw.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xgj.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pcf.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ntg.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://afy.ivvv.top

[J09] 时区处理
来源：http://bnm.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mxt.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rmk.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nmi.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mhq.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wjl.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://unf.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xrv.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xii.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://vcb.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fnn.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ian.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://imh.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mzn.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lrc.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://myz.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nqm.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wdu.birdmap.top

================================================================================
来源：http://ory.smart0.xyz

K. JSON 与序列化
来源：http://znp.aibaodan.cn

================================================================================
来源：http://pxo.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://aun.cucudq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gxc.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bpl.birdmap.top

JS:   JSON.stringify(obj)
来源：http://cwd.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://puv.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ege.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://szy.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://tgr.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sfs.havefunace.top

[K02] JSON 字符串转对象
来源：http://jad.chenlongwang.top

Py:   json.loads(s)
来源：http://snb.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qvo.hywenlv.cn

JS:   JSON.parse(s)
来源：http://kts.jianghu66.top

TS:   JSON.parse(s)
来源：http://fjh.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qps.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ffz.c1oappe.top

Ruby: JSON.parse(s)
来源：http://xjk.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uqe.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://nif.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ihi.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sqe.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rrr.shuidangran.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kzk.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ajz.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pxg.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://brb.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oih.zdqjudy.top

[K04] 读取 JSON 文件
来源：http://bpm.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://upj.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rzz.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qej.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://goa.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qbm.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://teu.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://dvt.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rey.jyoumei.cn

[K05] 深拷贝对象
来源：http://aqg.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://nfq.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://slk.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://xur.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://zgy.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://cqj.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zoq.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xcn.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bhf.gzhubu.top

[K06] 解析 URL 查询串
来源：http://wxv.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tia.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fqo.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qsg.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://llp.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://svo.52xcode.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iof.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lgu.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fht.hnxiangtu.top

[K07] 进制转换
来源：http://tbv.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ydu.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qkg.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lfc.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://crq.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vqv.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kcc.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://khz.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wiv.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://iut.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://xto.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kzu.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://hha.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://nry.jinqigfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yvz.0kj1m.cn

Go:   encoding/gob
来源：http://fld.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://zko.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bcb.jiagoushi.top

================================================================================
来源：http://htf.yongpay.top

L. 网络请求
来源：http://zoq.hammf.cn

================================================================================
来源：http://ksl.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://eyp.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wwg.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rom.zhijiandao.cn

JS:   await fetch(url)
来源：http://eoa.snrcjt.cn

TS:   await fetch(url)
来源：http://ppm.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://duq.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://xio.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://brc.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xgw.zhixingplan.top

[L02] 发送 POST JSON
来源：http://pea.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://yme.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qbc.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kgm.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nki.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qqd.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mxe.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zqp.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nab.cdnleiting.top

[L03] 设置自定义请求头
来源：http://xmn.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xxe.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qmr.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://noa.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oab.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ekh.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ppz.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vfe.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jih.zhengqikj.top

[L04] 设置超时
来源：http://cfb.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://oco.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eed.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dra.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mcj.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bcs.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jyy.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tmn.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rfm.316326.xyz

[L05] 上传文件（multipart）
来源：http://vka.yj20258888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qon.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sbw.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dxs.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cqw.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://omp.xingfuxueyuan.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zpa.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sow.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://diu.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://pqk.gzhubu.top

Py:   resp.json()
来源：http://byb.xinyue.icu

PHP:  json_decode($body, true);
来源：http://swz.xylfe.cn

JS:   await resp.json()
来源：http://prk.gaohongyu789.top

TS:   await resp.json()
来源：http://ehw.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nta.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fxg.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://etf.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aaw.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://okl.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eka.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sei.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://zwf.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://wea.hammf.cn

Java: resp.statusCode()
来源：http://tsk.dianchejie.cn

Go:   resp.StatusCode
来源：http://yli.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://nrz.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://bfn.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://cnn.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ekd.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://xts.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vhx.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://joh.zhengqikj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://keq.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vpm.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qst.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://alz.sjlbkw.cn

================================================================================
来源：http://fiu.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://uam.xziqi.cn

================================================================================
来源：http://klz.gogol.net.cn

[M01] 读取命令行参数
来源：http://nfq.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://zqe.fktsv.cn

PHP:  $argv;  $argc;
来源：http://xwk.redwolf501.top


<!-- 参考信息 -->