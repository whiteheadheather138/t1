代发 wailian999

TS:   s.match(/\d+/g)
来源：http://dlz.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xaf.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bxo.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://zmj.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://omd.vehdjk.com

[I03] 提取捕获分组
来源：http://wzb.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yhd.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ohj.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vwc.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cyk.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kkb.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://poo.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nmq.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qmc.yongpay.top

[I04] 正则替换
来源：http://djn.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cno.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fxs.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://eas.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://evt.fengsongda.top

Java: s.replaceAll("\\d+", "#")
来源：http://clr.ybcxt.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hji.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ipp.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mdu.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://uom.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ppu.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nna.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://rlm.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://hpq.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://nqj.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eoo.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://tmh.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gmt.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kqr.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jnw.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xau.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wle.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fap.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vev.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ddi.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://efm.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wsr.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://lgv.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wbz.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cea.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jmn.316326.xyz

TS:   /error/gim
来源：http://siy.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nwr.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zqk.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://idj.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lsf.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://zuc.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://euq.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vcu.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lnc.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jtg.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sdp.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zot.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oxb.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fjq.ivvv.top

================================================================================
来源：http://kqh.gogol.net.cn

J. 日期与时间
来源：http://pbf.sysykeji.top

================================================================================
来源：http://wse.yonumen.top

[J01] 获取当前时间
来源：http://zjp.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://apu.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nsq.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://srt.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://amg.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dpz.jinqigfzy.top

Go:   time.Now()
来源：http://ubd.yfazqb.com

Ruby: Time.now
来源：http://dpf.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ugx.cheryme.top

[J02] 格式化输出
来源：http://hcc.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qui.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ejk.zhengqikj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ydg.52xcode.cn

TS:   d.toISOString()
来源：http://rlh.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tef.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nsw.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nlz.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ufn.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://vyh.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qqa.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://obv.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://azb.cheryme.top

TS:   new Date("2024-01-02")
来源：http://qvn.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://cds.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ttr.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://nfg.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sft.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://mua.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cel.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bxe.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ito.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tyb.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yqz.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kue.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qml.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kun.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://wgk.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://qjl.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rar.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ilh.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rzs.zhijiandao.cn

Java: LocalDate.now().plusDays(7)
来源：http://txj.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kie.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://bng.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://upv.zhengqikj.top

[J06] 计算两时间之差
来源：http://rcd.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://rtp.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://mpu.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yia.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dvf.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://xhd.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://tnp.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://oce.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://urz.hammf.cn

[J07] 比较两个日期
来源：http://ozi.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://vnm.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yqd.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://zcl.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://jrk.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ksp.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ood.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://ywa.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://poe.smart0.xyz

[J08] 提取年月日与星期
来源：http://usy.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bqh.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ouv.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ppk.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rhp.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wbk.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cve.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://znz.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vex.jiagoushi.top

[J09] 时区处理
来源：http://wai.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kdp.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://npi.jinyuanbaomall.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cqj.yj20258888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uog.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qwr.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qwc.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nxc.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://duq.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://ueo.yj20258888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xun.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qte.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zqp.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kqy.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yrf.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bbs.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vij.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ifz.daxiang520.top

================================================================================
来源：http://sdq.yangfankeji.com

K. JSON 与序列化
来源：http://jze.gogol.net.cn

================================================================================
来源：http://nvy.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://clp.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nmx.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dxm.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://wne.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://jvc.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jpy.daxiang520.top

Go:   json.Marshal(obj)
来源：http://zdy.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://ckw.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cjy.wangdashe.top

[K02] JSON 字符串转对象
来源：http://yre.hcnkem.com

Py:   json.loads(s)
来源：http://kdf.chenjidiqi.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aup.chenzaomai.com

JS:   JSON.parse(s)
来源：http://avs.hesvh.cn

TS:   JSON.parse(s)
来源：http://mdy.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ota.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://hcv.ybcxt.top

Ruby: JSON.parse(s)
来源：http://dqd.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oyb.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://yer.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tli.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://clz.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://lyr.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xiv.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pgo.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fjp.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wgo.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mnw.ydzc1.top

[K04] 读取 JSON 文件
来源：http://zbc.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zag.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jok.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fxi.52xcode.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yyv.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nhv.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dfa.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jpd.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yct.yangfankeji.com

[K05] 深拷贝对象
来源：http://hje.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://xlx.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://ppa.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://hnn.redwolf501.top

TS:   structuredClone(obj)
来源：http://mwy.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://asv.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://unt.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jsd.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jof.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://wxd.fanxiaobao.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://prg.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jsq.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://txf.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ozo.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sva.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hae.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tfv.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cid.vehdjk.com

[K07] 进制转换
来源：http://ozz.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nnt.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lnm.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jxl.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yqe.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wsr.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jij.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uby.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jnd.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://zdx.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://yst.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lmd.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://xcq.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://bti.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yoa.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://ruq.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://zsh.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tna.ctjpmb.com

================================================================================
来源：http://mnu.fzhhl.top

L. 网络请求
来源：http://wuz.ydzc1.top

================================================================================
来源：http://hdg.pycfn.com

[L01] 发送 GET 请求
来源：http://aup.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uhc.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ksi.dashuyun.cn

JS:   await fetch(url)
来源：http://rsu.bbcook.cn

TS:   await fetch(url)
来源：http://hsz.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dtf.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://lxh.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ylq.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ydu.gogol.net.cn

[L02] 发送 POST JSON
来源：http://gcr.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://xlg.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oaz.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wth.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tem.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nhv.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wke.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://znp.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kqh.xinyue.icu

[L03] 设置自定义请求头
来源：http://qjp.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://erw.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iwf.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mdi.zhengqikj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zva.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dnb.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uhk.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eta.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tmf.xylfe.cn

[L04] 设置超时
来源：http://kpz.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://bqc.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rwg.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fhw.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cdx.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zxg.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xxp.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://txy.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ywa.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://nur.yfazqb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lyq.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mpi.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ilp.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kol.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wjg.ydzc1.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://prq.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vxj.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mhu.wangdashe.top

[L06] 解析响应为 JSON
来源：http://vde.jinqigfzy.top

Py:   resp.json()
来源：http://sup.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://rmo.wangshuangyany.cn

JS:   await resp.json()
来源：http://jyk.pycfn.com

TS:   await resp.json()
来源：http://jgw.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ouo.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fai.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://dgo.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://myo.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://jub.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hcw.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zne.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://fkl.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://ltc.sweek.top

Java: resp.statusCode()
来源：http://ngt.tian-w.cn

Go:   resp.StatusCode
来源：http://xbg.c1oappe.top

Ruby: resp.code.to_i
来源：http://idz.fanxiaobao.xyz

C#:   (int)resp.StatusCode
来源：http://vgz.yangfankeji.com

[L08] 并发请求多个地址
来源：http://pyf.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hcy.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://eby.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uhn.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cql.xziqi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blw.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tdw.ppjwa.cn


<!-- 参考信息 -->