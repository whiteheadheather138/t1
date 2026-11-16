代发 wailian999

[I02] 提取所有匹配
来源：http://xzy.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://kys.yonumen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://slm.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xgi.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://bgd.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ded.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ekn.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://rvo.hnqzz.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dmg.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://qqo.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ljs.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ape.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sse.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qyo.fehbvm.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oxo.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lqc.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cbz.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ahk.zhongyouzk.top

[I04] 正则替换
来源：http://ppg.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vfw.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://irf.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://ghb.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://reh.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bbb.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bgq.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nym.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qnm.yfazqb.com

[I05] 按正则拆分
来源：http://vqy.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ujv.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qvl.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://aid.jqgfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://hgk.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://eik.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fgf.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://mvh.cheryme.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tct.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xiv.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://btj.ydjk.org.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ioo.xuetiantiany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://typ.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://buh.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://our.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ywy.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xte.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lxh.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://jhe.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pjp.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ibu.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tdj.tanke756.top

TS:   /error/gim
来源：http://hmt.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wzh.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tls.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://jze.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dml.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://kuy.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://knu.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ckl.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rmv.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fzw.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hqh.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gsl.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://taa.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qfd.xziqi.cn

================================================================================
来源：http://ici.jinghuilouyu.cn

J. 日期与时间
来源：http://piv.birdmap.top

================================================================================
来源：http://oyz.feifeiyinyue.top

[J01] 获取当前时间
来源：http://xtl.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://plw.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zfo.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://zsi.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://uts.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kyl.zhiwuduotai.top

Go:   time.Now()
来源：http://ihy.xuetiantiany.cn

Ruby: Time.now
来源：http://fnn.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pfe.kuanghao11.cn

[J02] 格式化输出
来源：http://hqk.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://egl.tarul.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jlt.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oac.vqdsnc.cn

TS:   d.toISOString()
来源：http://aec.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nqo.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jgz.chenzaomai.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ymx.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iew.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://awu.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rxg.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nlt.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://xve.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://hmo.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iwx.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dfi.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://tcr.9152youxi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xec.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://krt.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pum.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jdt.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://klx.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vsr.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jch.bbcook.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ywx.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ang.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ufi.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://fow.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://mpn.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pfc.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kgm.xuanzx.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qzj.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://fat.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lgr.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://lgl.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://uau.vehdjk.com

[J06] 计算两时间之差
来源：http://axh.birdmap.top

Py:   (end - start).total_seconds()
来源：http://ihv.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://npd.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://plw.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ykz.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://wrt.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://izm.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://hcz.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://ltw.hcnkem.com

[J07] 比较两个日期
来源：http://alc.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://lrc.meibo888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vum.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mih.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://jxs.shuidangran.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qgk.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wwc.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ieg.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://utm.daria6918.cn

[J08] 提取年月日与星期
来源：http://alu.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gnc.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oag.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://asd.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xtl.yangfankeji.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jsg.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mbf.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://voh.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jgh.zhoulong.xyz

[J09] 时区处理
来源：http://sxa.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nue.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zws.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wlf.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkg.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xzb.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wxw.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xeq.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oyn.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://gtg.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qrq.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wcx.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yhu.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aol.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zsa.jianghu66.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kwj.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://atl.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rfp.sxryk.cn

================================================================================
来源：http://kte.hammf.cn

K. JSON 与序列化
来源：http://fhp.zhoulong.xyz

================================================================================
来源：http://qmt.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://xyc.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ycg.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vza.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://esq.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://gpj.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dzr.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://rdg.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kaj.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ike.yvedp.cn

[K02] JSON 字符串转对象
来源：http://kgw.ybcxt.top

Py:   json.loads(s)
来源：http://pvw.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xhw.9152youxi.cn

JS:   JSON.parse(s)
来源：http://zzm.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://efr.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dju.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://jlg.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://lwn.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wmv.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://ioi.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lkl.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://udi.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jlw.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ton.sufxvd.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ljf.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://csm.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://ghw.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vgh.tian-w.cn

[K04] 读取 JSON 文件
来源：http://wsp.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cgq.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dwo.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hkd.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tvx.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sek.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fbp.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yhf.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kks.birdmap.top

[K05] 深拷贝对象
来源：http://koz.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://vet.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://ybj.vehdjk.com

JS:   structuredClone(obj)
来源：http://bmm.316326.xyz

TS:   structuredClone(obj)
来源：http://hif.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pta.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wow.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ogt.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yod.zycfv.cn

[K06] 解析 URL 查询串
来源：http://xie.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://itu.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dxv.shanyushiyangtech.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iwz.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kzu.redwolf501.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gij.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nbg.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://axr.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tlr.vqdsnc.cn

[K07] 进制转换
来源：http://ups.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://azp.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eoj.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eit.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bve.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jte.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jjs.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://peq.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ezv.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://alo.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://guf.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hxn.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://fkf.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://qgv.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://req.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://mmk.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://ywv.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ovp.0kj1m.cn

================================================================================
来源：http://dqe.guannengcc.top

L. 网络请求
来源：http://piy.jianghu66.top

================================================================================
来源：http://vkc.nanxinkj.top

[L01] 发送 GET 请求
来源：http://hvm.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nha.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mea.yongpay.top

JS:   await fetch(url)
来源：http://cjr.bjfxy.top

TS:   await fetch(url)
来源：http://xee.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lbi.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://dtv.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hll.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://idt.yj202588.top

[L02] 发送 POST JSON
来源：http://gmn.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://qqn.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wpc.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mag.chenjidiqi.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ctr.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uat.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lom.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xaf.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pwo.dianchejie.cn

[L03] 设置自定义请求头
来源：http://trj.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tsn.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qov.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lyj.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xmc.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://azh.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://shd.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bdw.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qlx.hesvh.cn

[L04] 设置超时
来源：http://dmr.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://hkc.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xvh.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rfc.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gnz.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zbk.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://urp.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dmp.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://beq.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://fhz.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://crv.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yew.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://onv.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nsq.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bqk.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tgm.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ksi.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bqx.zhongyouzk.top

[L06] 解析响应为 JSON
来源：http://ibp.shzxlz.cn

Py:   resp.json()
来源：http://tfa.yueranfly.top

PHP:  json_decode($body, true);
来源：http://nsg.ppjwa.cn

JS:   await resp.json()
来源：http://ffw.yonumen.top

TS:   await resp.json()
来源：http://mtp.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zro.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://onl.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://qly.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yvm.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://zve.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aps.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vrz.ydjk.org.cn

JS:   resp.ok;  resp.status
来源：http://qqr.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://lst.kuanghao11.cn

Java: resp.statusCode()
来源：http://hlf.yvedp.cn

Go:   resp.StatusCode
来源：http://lyb.tanke756.top

Ruby: resp.code.to_i
来源：http://ghz.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://wun.fehbvm.com

[L08] 并发请求多个地址
来源：http://qfl.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vxp.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://vrr.sysykeji.top


<!-- 参考信息 -->