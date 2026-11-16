代发 wailian999

TS:   s.match(/\d+/g)
来源：http://vws.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nly.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pcb.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://mpj.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gnm.shzxlz.cn

[I03] 提取捕获分组
来源：http://blz.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dqq.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gsl.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gsc.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cdx.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ovx.cdnleiting.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jej.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uhg.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kzj.ctjpmb.com

[I04] 正则替换
来源：http://uvq.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://kog.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qae.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cms.yongpay.top

TS:   s.replace(/\d+/g, "#")
来源：http://qrq.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kaj.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bon.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kqs.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xby.zhengqikj.top

[I05] 按正则拆分
来源：http://aal.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ssa.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dfw.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://yvf.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://jwi.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://zno.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ipj.nanxuanxn.top

Ruby: s.split(/\s*,\s*/)
来源：http://bnk.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gtd.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://beh.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rkp.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sbd.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eit.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bfx.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ofa.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://clo.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://moj.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oge.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://mnq.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xfw.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bsx.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nld.meibo888.top

TS:   /error/gim
来源：http://yep.zhongyouzk.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bld.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hru.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://jgb.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://piu.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://tpu.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://enx.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://elr.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gvq.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vdi.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kjc.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hor.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dcg.ivvv.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://phz.hnxiangtu.top

================================================================================
来源：http://wdz.9152youxi.cn

J. 日期与时间
来源：http://tfg.bbcook.cn

================================================================================
来源：http://phf.c1oappe.top

[J01] 获取当前时间
来源：http://fba.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lhh.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ygu.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://vzk.iojbl.cn

TS:   new Date();  Date.now()
来源：http://aga.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://sep.tarul.cn

Go:   time.Now()
来源：http://blt.bjfxy.top

Ruby: Time.now
来源：http://krf.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://frf.zhongyouzk.top

[J02] 格式化输出
来源：http://vkb.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vyo.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nps.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rwm.wangshuangyany.cn

TS:   d.toISOString()
来源：http://mnt.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rny.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ndd.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uwh.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fyt.jyoumei.cn

[J03] 字符串解析为日期
来源：http://xov.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://joz.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kru.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://alz.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://fby.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://lat.hnqzz.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vid.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://psx.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qzm.tian-w.cn

[J04] 时间戳与日期互转
来源：http://eku.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://meh.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tou.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ndt.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vuv.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bnj.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://weo.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tew.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tec.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://hqa.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://neb.shangyingyoupin.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rbq.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cfv.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mzy.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://ynb.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wmw.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://pmh.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://cpq.hammf.cn

[J06] 计算两时间之差
来源：http://msc.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://igp.yfazqb.com

PHP:  $end->diff($start)->days;
来源：http://oxr.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qse.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://due.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://mpw.yuxming.cn

Go:   end.Sub(start).Hours()
来源：http://dir.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://pmi.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://grd.daxiang520.top

[J07] 比较两个日期
来源：http://irr.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://pxz.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://scb.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ctf.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://tmx.shuidangran.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://epq.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nsb.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ywj.c1oappe.top

C#:   d1 < d2;  d1 == d2
来源：http://hvv.zycfv.cn

[J08] 提取年月日与星期
来源：http://rae.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://epy.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rnw.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yfs.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kpp.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yrl.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://woe.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rho.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fbs.andypj.xyz

[J09] 时区处理
来源：http://tmv.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nnh.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ycz.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jbn.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uph.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ixf.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://psi.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://umh.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tvu.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://iro.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lkd.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wsm.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ptq.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qps.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oie.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lzt.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ojb.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wqh.bbcook.cn

================================================================================
来源：http://ryq.snrcjt.cn

K. JSON 与序列化
来源：http://uee.hysaishi.cn

================================================================================
来源：http://yhi.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://huq.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yto.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cfd.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://mhz.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://unj.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iaz.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://wwo.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://vhg.ppjwa.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pwd.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://ylr.sjlbkw.cn

Py:   json.loads(s)
来源：http://yyk.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lxq.haohaochexian.top

JS:   JSON.parse(s)
来源：http://zla.sufxvd.cn

TS:   JSON.parse(s)
来源：http://rpi.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zki.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://ota.ydzc1.top

Ruby: JSON.parse(s)
来源：http://kdf.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eeg.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://yrx.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tgz.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ezk.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qur.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://kkx.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://amo.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uxj.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dsg.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vdg.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://svk.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kwi.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ump.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://trj.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dxz.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gwb.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://alk.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vmw.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uuf.cucudq.cn

[K05] 深拷贝对象
来源：http://fhr.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://wmm.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://etn.smart0.xyz

JS:   structuredClone(obj)
来源：http://poo.jianghu66.top

TS:   structuredClone(obj)
来源：http://veu.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pys.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://frc.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xox.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://cdy.yfazqb.com

[K06] 解析 URL 查询串
来源：http://eig.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dvw.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ufz.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jae.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tvo.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vjo.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://xuk.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ejj.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pve.jlsjyb.cn

[K07] 进制转换
来源：http://awo.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zpk.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://umw.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ras.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qqi.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mzm.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wqo.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://csx.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ytc.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://oqy.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://xnm.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qia.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://use.ydjk.org.cn

TS:   v8.serialize(obj)        // Node
来源：http://moo.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ypa.hnqzz.top

Go:   encoding/gob
来源：http://xqi.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://tcz.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gli.birdmap.top

================================================================================
来源：http://fre.tian-w.cn

L. 网络请求
来源：http://vff.fengsongda.top

================================================================================
来源：http://afe.gotoacloud.top

[L01] 发送 GET 请求
来源：http://oib.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vzl.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://meg.gotoacloud.top

JS:   await fetch(url)
来源：http://qyg.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://uif.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yeo.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://jxw.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dzc.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dhy.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://lmj.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://gta.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hql.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wtb.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kgq.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hqh.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qjq.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qyo.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bhy.bjfxy.top

[L03] 设置自定义请求头
来源：http://qcx.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://csr.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yoa.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bej.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qge.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rat.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lob.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rhk.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yed.0kj1m.cn

[L04] 设置超时
来源：http://ldr.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://vaq.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xos.cqqwz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://omo.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://owk.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ovn.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://anq.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sbm.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rrs.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://fvt.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qzu.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wah.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eiv.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tiy.ydzc1.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ykq.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://svf.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qdr.xingfuxueyuan.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lld.xylfe.cn

[L06] 解析响应为 JSON
来源：http://imc.jinghuilouyu.cn

Py:   resp.json()
来源：http://ipu.bbcook.cn

PHP:  json_decode($body, true);
来源：http://mkb.xinyue.icu

JS:   await resp.json()
来源：http://pnz.wangshuangyany.cn

TS:   await resp.json()
来源：http://ozj.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yvc.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vem.zhongyouzk.top

Ruby: JSON.parse(resp.body)
来源：http://kvm.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yyn.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://lva.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wfy.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ntr.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://voy.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://ppe.zhongyouzk.top

Java: resp.statusCode()
来源：http://bld.9152youxi.cn

Go:   resp.StatusCode
来源：http://amt.xziqi.cn

Ruby: resp.code.to_i
来源：http://hwt.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://zst.uphjek.com

[L08] 并发请求多个地址
来源：http://vtj.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cdn.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://ydc.zhaomingkeji.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fpq.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qzd.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jcp.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xcd.tianlin.xyz


<!-- 参考信息 -->