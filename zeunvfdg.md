代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jhe.jqgfzy.top

[I03] 提取捕获分组
来源：http://blo.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ctf.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://anw.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qxq.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nlq.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mbu.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pzv.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wzf.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pzk.bbcook.cn

[I04] 正则替换
来源：http://bva.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mmm.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vxr.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://val.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://bco.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://dwz.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pny.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://hjg.gotoacloud.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pik.uphjek.com

[I05] 按正则拆分
来源：http://qew.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qpk.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rmm.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://bro.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://knh.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://rwm.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wjv.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://fst.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zdb.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vkk.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bie.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pyk.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://odp.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://arl.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zti.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://law.ybcxt.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ijg.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zek.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://yig.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fpr.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dfk.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sqj.andypj.xyz

TS:   /error/gim
来源：http://abp.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wqi.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aqo.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://ztf.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qve.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://wlf.hcnkem.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mwj.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zvl.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jhc.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zqm.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sgc.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gob.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fzs.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iaq.chenzaomai.com

================================================================================
来源：http://uma.andypj.xyz

J. 日期与时间
来源：http://fyt.yfazqb.com

================================================================================
来源：http://vuq.yuanzhike.top

[J01] 获取当前时间
来源：http://esv.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://eqm.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eiz.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://fwp.yvedp.cn

TS:   new Date();  Date.now()
来源：http://xgf.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://kwt.fanxiaobao.xyz

Go:   time.Now()
来源：http://wpe.xziqi.cn

Ruby: Time.now
来源：http://nbm.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://srg.tarul.cn

[J02] 格式化输出
来源：http://gip.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jtm.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bls.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ztg.svipenyu.cn

TS:   d.toISOString()
来源：http://bbl.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lij.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zlh.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qfs.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://byi.52xcode.cn

[J03] 字符串解析为日期
来源：http://izj.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bhg.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://upq.pycfn.com

JS:   new Date("2024-01-02")
来源：http://yba.birdmap.top

TS:   new Date("2024-01-02")
来源：http://sce.xylfe.cn

Java: LocalDate.parse("2024-01-02")
来源：http://huv.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tiw.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://gpw.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oci.fehbvm.com

[J04] 时间戳与日期互转
来源：http://skg.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kyd.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://njb.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lrp.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pid.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qho.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zrg.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kmt.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://koq.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://jck.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://mzh.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://utd.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ifs.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mdx.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://xuy.hesvh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://thk.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://thc.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://aqs.xuanzx.com

[J06] 计算两时间之差
来源：http://mad.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://oax.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://byu.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://keq.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pun.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://dxo.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://kvn.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://fnv.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://fjs.ehwqpu.com

[J07] 比较两个日期
来源：http://mve.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://gnp.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://spt.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://tne.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://jgl.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dye.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://weq.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://kvp.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://coe.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://pzh.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ptk.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qxq.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lsc.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rkj.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zbq.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ltr.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bmp.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wnf.zhaomingkeji.xyz

[J09] 时区处理
来源：http://nxl.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pyg.hnqzz.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vii.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vhs.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uow.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xhh.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ars.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wxf.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hyi.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://gzm.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rso.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ffv.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oug.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jns.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lrg.ybcxt.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dnv.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rbs.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dsu.havefunace.top

================================================================================
来源：http://ilz.daria6918.cn

K. JSON 与序列化
来源：http://iqo.cashguo.top

================================================================================
来源：http://izi.zhijiandao.cn

[K01] 对象转 JSON 字符串
来源：http://smw.fktsv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lxm.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dlf.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://ehs.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://pfw.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kaq.yonumen.top

Go:   json.Marshal(obj)
来源：http://pqo.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lmd.hesvh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xek.52xcode.cn

[K02] JSON 字符串转对象
来源：http://mrq.jqgfzy.top

Py:   json.loads(s)
来源：http://pmq.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kqu.ybcxt.top

JS:   JSON.parse(s)
来源：http://qed.hywenlv.cn

TS:   JSON.parse(s)
来源：http://uze.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rnd.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://xvi.meibo888.top

Ruby: JSON.parse(s)
来源：http://hfz.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bqc.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://ddq.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://btl.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qxw.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gnv.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nna.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vuz.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oom.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xwe.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://asv.yj202588.top

[K04] 读取 JSON 文件
来源：http://kqb.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vxr.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hom.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vee.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xxd.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://knw.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fbx.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rya.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wvx.tanke756.top

[K05] 深拷贝对象
来源：http://alx.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://fxu.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://ird.guannengcc.top

JS:   structuredClone(obj)
来源：http://vmk.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://ivc.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://pke.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vad.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vvh.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://dfs.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://nos.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vyf.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rai.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://asy.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ogg.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qrj.yj20258.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mai.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://otl.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ofk.ivvv.top

[K07] 进制转换
来源：http://vrf.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wdj.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vjg.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://scy.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://swd.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cwi.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cnq.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xuq.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oir.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://urb.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://zik.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wrt.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://uis.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://gyz.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ohf.chenlongwang.top

Go:   encoding/gob
来源：http://dih.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://tke.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ysw.hesvh.cn

================================================================================
来源：http://mmk.ehwqpu.com

L. 网络请求
来源：http://elj.vehdjk.com

================================================================================
来源：http://iio.cucudq.cn

[L01] 发送 GET 请求
来源：http://stv.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tpc.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sop.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://rsb.ehwqpu.com

TS:   await fetch(url)
来源：http://ufz.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xbz.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://ddx.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gkn.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kqz.jianghu66.top

[L02] 发送 POST JSON
来源：http://irk.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://asn.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tpu.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://voa.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qzl.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qmj.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qgu.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zqr.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yrs.xinyue.icu

[L03] 设置自定义请求头
来源：http://erk.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qax.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ope.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://syi.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vhm.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zrq.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hpc.kuanghao11.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rqf.gaohongyu789.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://neq.gaohongyu789.top

[L04] 设置超时
来源：http://jcz.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://kfj.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eaf.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tqr.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxt.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hkr.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mgx.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gum.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zoa.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://ayj.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qoo.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zst.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vpm.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tqo.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mzz.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rma.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hqp.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ovm.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://zms.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://khj.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://icq.316326.xyz

JS:   await resp.json()
来源：http://bpv.zdqjudy.top

TS:   await resp.json()
来源：http://ksm.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://row.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xdk.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://rms.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xmb.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://dbc.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dtn.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nhh.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://xtt.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://fuy.iojbl.cn

Java: resp.statusCode()
来源：http://ndo.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://vhs.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://mku.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://ehw.tarul.cn

[L08] 并发请求多个地址
来源：http://zfm.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fgr.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://dxp.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bgg.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qtz.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wnt.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sra.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://khf.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hag.fzhhl.top

================================================================================
来源：http://ypg.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://hir.jinyuanbaomall.cn


<!-- 参考信息 -->