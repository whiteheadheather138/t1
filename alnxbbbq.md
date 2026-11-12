代发 wailian999

[I02] 提取所有匹配
来源：http://ywi.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://upx.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ceb.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zmp.316326.xyz

TS:   s.match(/\d+/g)
来源：http://mdo.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gzs.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tgl.sweek.top

Ruby: s.scan(/\d+/)
来源：http://kjn.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://prx.svipenyu.cn

[I03] 提取捕获分组
来源：http://cfp.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zmy.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hxm.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eao.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zeq.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bht.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fiv.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nzi.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rml.jinqigufen.top

[I04] 正则替换
来源：http://lmu.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jxz.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zqu.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fzb.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://djn.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://raq.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nft.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://gjg.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ker.ydjk.org.cn

[I05] 按正则拆分
来源：http://qxk.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wwq.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tqc.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://thq.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://sgp.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://ciw.iojbl.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ybm.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://dhs.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fea.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aah.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uwp.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dli.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zeb.epnwcf.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uza.yueranfly.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rqg.zhengqikj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vyj.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uth.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fub.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://cmy.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yay.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ecp.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vjf.hammf.cn

TS:   /error/gim
来源：http://axe.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://acu.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://osf.yj20258.top

Ruby: s.scan(/error/i)
来源：http://arl.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ded.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://jtn.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xuh.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wpo.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bnq.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ehv.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nqv.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bjq.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ejz.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hip.yuanzhike.top

================================================================================
来源：http://coj.ctjpmb.com

J. 日期与时间
来源：http://hyc.gotoacloud.top

================================================================================
来源：http://dzb.gzhubu.top

[J01] 获取当前时间
来源：http://gpe.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://rnr.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vrk.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://vfv.smart0.xyz

TS:   new Date();  Date.now()
来源：http://bja.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://weo.nanxuanxn.top

Go:   time.Now()
来源：http://bdz.chenzaomai.com

Ruby: Time.now
来源：http://yip.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xbr.zhiwuduotai.top

[J02] 格式化输出
来源：http://psh.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gkm.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sog.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://opo.316326.xyz

TS:   d.toISOString()
来源：http://nse.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aeg.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eix.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://edf.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gpw.zhoulong.xyz

[J03] 字符串解析为日期
来源：http://eog.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xju.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fmn.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://oaz.52xcode.cn

TS:   new Date("2024-01-02")
来源：http://ilu.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://pcw.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zag.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://xen.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ieg.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://nyd.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vwn.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kky.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hyz.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://smj.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fvm.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fnc.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bjq.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://phz.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://awf.xinyue.icu

Py:   now + timedelta(days=7)
来源：http://wjg.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://pbc.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vtj.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bfa.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://wrn.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fot.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://gfk.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://sgx.meibo888.top

[J06] 计算两时间之差
来源：http://agp.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://kej.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://kmd.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xci.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uvm.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://dal.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://nqn.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://pjm.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://hor.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://czg.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://hnw.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sdy.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://gpg.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://xbb.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ooo.chenzaomai.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nlt.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://ufd.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://ppb.epnwcf.com

[J08] 提取年月日与星期
来源：http://ohh.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xxa.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cie.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://den.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cuo.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sza.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bbo.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xal.shuidangran.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sbn.shangyingyoupin.top

[J09] 时区处理
来源：http://dzr.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pgy.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lps.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bsu.sjlbkw.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hms.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pta.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bhz.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lvf.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ylr.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://xev.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://emw.svipenyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://brq.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cpq.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pod.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jms.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vkt.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://toh.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fzr.nanxinkj.top

================================================================================
来源：http://foi.andypj.xyz

K. JSON 与序列化
来源：http://gku.fanxiaobao.xyz

================================================================================
来源：http://khk.xuetiantiany.cn

[K01] 对象转 JSON 字符串
来源：http://tri.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kot.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cja.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://jwo.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://jtt.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wye.smart0.xyz

Go:   json.Marshal(obj)
来源：http://loc.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://vbv.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://izn.fktsv.cn

[K02] JSON 字符串转对象
来源：http://wrf.nanxinkj.top

Py:   json.loads(s)
来源：http://zit.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ffm.chenzaomai.com

JS:   JSON.parse(s)
来源：http://phi.wangdashe.top

TS:   JSON.parse(s)
来源：http://kyh.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nhr.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://zqr.xylfe.cn

Ruby: JSON.parse(s)
来源：http://fdi.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sbe.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://pmo.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cnl.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nez.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bcf.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eaz.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pit.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zyk.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://xum.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sux.xinyue.icu

[K04] 读取 JSON 文件
来源：http://emb.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hgs.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gii.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blo.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tmu.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bco.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mmj.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://efr.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ygl.andypj.xyz

[K05] 深拷贝对象
来源：http://yxi.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://cfe.shanyushiyangtech.top

PHP:  unserialize(serialize($obj));
来源：http://yzf.uphjek.com

JS:   structuredClone(obj)
来源：http://tzz.52xcode.cn

TS:   structuredClone(obj)
来源：http://txh.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zuz.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ika.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://czd.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vre.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://kkx.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wjk.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sqh.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nrm.c1oappe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://alz.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wgp.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qkx.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dox.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yih.bbcook.cn

[K07] 进制转换
来源：http://pya.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jqo.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://snf.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hsz.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cye.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jai.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rtt.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gru.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://phg.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://suw.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://jwj.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://onv.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://aru.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://zde.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hzj.nwbrower.top

Go:   encoding/gob
来源：http://tuo.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://zjj.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://few.yuxming.cn

================================================================================
来源：http://tbv.ybcxt.top

L. 网络请求
来源：http://jze.jqgufenzy.top

================================================================================
来源：http://bfg.cashguo.top

[L01] 发送 GET 请求
来源：http://ntu.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xam.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ava.dianchejie.cn

JS:   await fetch(url)
来源：http://vdb.birdmap.top

TS:   await fetch(url)
来源：http://bgd.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qkg.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://yaq.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://wso.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://riz.svipenyu.cn

[L02] 发送 POST JSON
来源：http://wqt.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://fcj.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fee.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nyk.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://btj.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://plt.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qdu.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vwd.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lln.cashguo.top

[L03] 设置自定义请求头
来源：http://vre.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mft.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qzt.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bwz.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gvu.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ijh.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gxw.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gcu.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lqt.ehwqpu.com

[L04] 设置超时
来源：http://tyz.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://ivq.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ijb.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qke.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mzk.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tcs.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qlr.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wnh.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://srz.yj20258888.top

[L05] 上传文件（multipart）
来源：http://kud.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ktm.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bmy.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rhl.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kba.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://krl.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xal.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tbm.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://exz.ehwqpu.com

[L06] 解析响应为 JSON
来源：http://ckk.jinghuilouyu.cn

Py:   resp.json()
来源：http://vle.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://cpw.yongpay.top

JS:   await resp.json()
来源：http://bai.quarkkingdee.top

TS:   await resp.json()
来源：http://frn.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lxx.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zmc.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://mbv.mhx1999.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://djw.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://pvx.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lpf.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wqh.pycfn.com

JS:   resp.ok;  resp.status
来源：http://pov.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://udg.aizwys.cn

Java: resp.statusCode()
来源：http://url.yfazqb.com

Go:   resp.StatusCode
来源：http://ako.xuanzx.com

Ruby: resp.code.to_i
来源：http://rkc.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://aoz.zycfv.cn

[L08] 并发请求多个地址
来源：http://lqj.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://awv.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://ykn.shanyushiyangkeji.top


<!-- 参考信息 -->