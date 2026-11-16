代发 wailian999

TS:   s.match(/\d+/g)
来源：http://bxm.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rxz.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://col.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://kfx.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zqk.guannengcc.top

[I03] 提取捕获分组
来源：http://ncs.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hsb.yangfankeji.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bfm.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pty.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dhe.nanxuanxn.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://srn.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rdk.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ljf.ybcxt.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zjl.ehwqpu.com

[I04] 正则替换
来源：http://sbl.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eya.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wne.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://gje.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sev.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ipa.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ppz.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://syt.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gja.zhengqikj.top

[I05] 按正则拆分
来源：http://snu.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nsm.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bhi.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://iih.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://oup.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://qvj.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cps.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vlf.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://plw.pengpengdd.cyou

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gzu.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ylk.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cru.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://akg.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://trb.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gij.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mwn.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bjc.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vuy.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://fja.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://era.zdqjudy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dhf.guannengcc.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jdm.mhx1999.top

TS:   /error/gim
来源：http://oiu.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wbx.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hld.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://lev.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://apt.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://nza.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://smp.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wws.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kpv.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iph.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://zik.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eon.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kef.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iiu.tian-w.cn

================================================================================
来源：http://fxv.bjfxy.top

J. 日期与时间
来源：http://ket.yfazqb.com

================================================================================
来源：http://qnx.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://bgp.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hov.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tyg.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://xnb.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://ylg.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dbf.fehbvm.com

Go:   time.Now()
来源：http://pfb.tianlin.xyz

Ruby: Time.now
来源：http://fpa.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xus.cucudq.cn

[J02] 格式化输出
来源：http://ysu.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bvb.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vfn.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nqx.sysykeji.top

TS:   d.toISOString()
来源：http://qbd.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zbk.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cnk.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://myz.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://upe.hesvh.cn

[J03] 字符串解析为日期
来源：http://dnc.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eef.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aky.cashguo.top

JS:   new Date("2024-01-02")
来源：http://hld.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://ime.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://qna.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://haa.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://dbr.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://krs.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://eym.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qeu.hnxiangtu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://huk.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oxe.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qgz.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://njg.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iuw.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qba.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hkm.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://bam.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://ujf.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tin.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xqf.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://emp.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://ygf.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mrg.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://aym.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ndv.zycfv.cn

[J06] 计算两时间之差
来源：http://lff.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://ong.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://zyg.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kxh.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fng.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://dxo.tarul.cn

Go:   end.Sub(start).Hours()
来源：http://qcg.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://zeu.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://qqy.hcnkem.com

[J07] 比较两个日期
来源：http://pxw.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://zdr.zhoulong.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jgl.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://eph.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://dhu.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://itc.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dlk.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://asy.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://rpn.hywenlv.cn

[J08] 提取年月日与星期
来源：http://fyx.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fli.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rdm.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zpb.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aec.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://upc.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rod.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yig.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://svp.hysaishi.cn

[J09] 时区处理
来源：http://csd.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ixk.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ilo.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bdi.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gdv.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ham.fzhhl.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uzd.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xml.meibo888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mju.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://krh.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qeh.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://upj.svipenyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ora.xingfuxueyuan.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uvg.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jiz.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bvm.9152youxi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bao.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vbr.hesvh.cn

================================================================================
来源：http://dcs.feifeiyinyue.top

K. JSON 与序列化
来源：http://uah.chenjidiqi.icu

================================================================================
来源：http://pqh.gzhubu.top

[K01] 对象转 JSON 字符串
来源：http://mit.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wlt.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yij.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://wxd.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://kio.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dmg.nwbrower.top

Go:   json.Marshal(obj)
来源：http://hxc.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ido.hammf.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ntj.zhiwuduotai.top

[K02] JSON 字符串转对象
来源：http://xfy.uphjek.com

Py:   json.loads(s)
来源：http://vjm.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tyc.hywenlv.cn

JS:   JSON.parse(s)
来源：http://lct.hysaishi.cn

TS:   JSON.parse(s)
来源：http://czj.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lrf.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://dsm.smart0.xyz

Ruby: JSON.parse(s)
来源：http://hpk.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ihs.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://ggj.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qnr.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kyx.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ipo.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kva.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gdo.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xor.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://zfz.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gqv.ybcxt.top

[K04] 读取 JSON 文件
来源：http://etw.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hiy.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gcz.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://brb.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wiy.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oea.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uss.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ckw.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vab.smart0.xyz

[K05] 深拷贝对象
来源：http://gxl.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://uyo.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://mjq.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://kgm.yj20258888.top

TS:   structuredClone(obj)
来源：http://kne.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://drd.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jmh.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kqy.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ocd.daxiang520.top

[K06] 解析 URL 查询串
来源：http://itb.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sfi.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pnl.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ekp.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kwo.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dky.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://odp.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://omp.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pzb.ivvv.top

[K07] 进制转换
来源：http://hut.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lfb.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bqq.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fhr.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eti.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mus.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://npe.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ztt.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://loh.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://yvm.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://crg.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wwn.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://fsf.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://mfq.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ihc.hfpthk.cn

Go:   encoding/gob
来源：http://jgv.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://bdt.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dci.xziqi.cn

================================================================================
来源：http://wii.ppjwa.cn

L. 网络请求
来源：http://cie.shanyushiyangkeji.top

================================================================================
来源：http://kwn.dianchejie.cn

[L01] 发送 GET 请求
来源：http://koq.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://acw.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qde.52xcode.cn

JS:   await fetch(url)
来源：http://iat.tian-w.cn

TS:   await fetch(url)
来源：http://dfh.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://klc.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://fwf.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://egc.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yrg.andypj.xyz

[L02] 发送 POST JSON
来源：http://wob.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://gio.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tjv.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://glt.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ztc.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gvx.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://azc.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ixq.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://krl.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://jgq.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qcm.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pww.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bor.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bua.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ozp.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cak.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xpn.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fgx.zhengqikj.top

[L04] 设置超时
来源：http://eir.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://mlx.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qxr.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cix.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xct.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mli.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yne.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uda.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xwc.birdmap.top

[L05] 上传文件（multipart）
来源：http://zan.hfpthk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://has.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cjk.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pqw.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://enr.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tea.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kgx.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vrx.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ejz.bbcook.cn

[L06] 解析响应为 JSON
来源：http://rvx.zycfv.cn

Py:   resp.json()
来源：http://iyi.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://ori.tian-w.cn

JS:   await resp.json()
来源：http://rze.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://ioz.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gvs.yangfankeji.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rgn.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://rnp.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pod.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://kzq.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sij.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://njo.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://moe.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://hap.fzhhl.top

Java: resp.statusCode()
来源：http://kim.pycfn.com

Go:   resp.StatusCode
来源：http://gqx.sufxvd.cn

Ruby: resp.code.to_i
来源：http://fws.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://bdz.uphjek.com

[L08] 并发请求多个地址
来源：http://beu.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kpt.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://llo.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zvl.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mvw.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xtq.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cro.jianghu66.top


<!-- 参考信息 -->