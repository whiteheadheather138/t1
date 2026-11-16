代发 wailian999

[I02] 提取所有匹配
来源：http://tun.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://rrd.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dyd.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://haz.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://imq.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gjh.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pzx.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://rmk.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vhc.uphjek.com

[I03] 提取捕获分组
来源：http://gxo.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pdi.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ptf.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dfn.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vic.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tsi.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vju.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sos.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ebz.sysykeji.top

[I04] 正则替换
来源：http://ywv.zhoulong.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://cba.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sll.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://ttb.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zls.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://mgy.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://inl.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://raf.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sqj.jinqigfzy.top

[I05] 按正则拆分
来源：http://ytt.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://mjy.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qdv.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://nca.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://eir.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://zhb.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mvg.fengsongda.top

Ruby: s.split(/\s*,\s*/)
来源：http://eap.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dfc.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uki.sufxvd.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://knx.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oae.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mhf.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cci.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rzq.jinyuanbaomall.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://igc.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hid.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://roy.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://fpk.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mni.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uym.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jfu.mhx1999.top

TS:   /error/gim
来源：http://yyp.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nby.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://env.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://rfi.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hjv.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://wxe.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bxt.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mcy.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://agc.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oht.daxiang520.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jpy.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aur.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gzz.52xcode.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ark.yuxming.cn

================================================================================
来源：http://uuw.pycfn.com

J. 日期与时间
来源：http://cyb.vqdsnc.cn

================================================================================
来源：http://jnm.kuanghao11.cn

[J01] 获取当前时间
来源：http://qpx.xinyue.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://ajp.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dox.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://sak.yanxiufei.cn

TS:   new Date();  Date.now()
来源：http://efk.xuanzx.com

Java: LocalDateTime.now();  Instant.now()
来源：http://aml.jqgufenzy.top

Go:   time.Now()
来源：http://yqt.jlsjyb.cn

Ruby: Time.now
来源：http://etq.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pep.hesvh.cn

[J02] 格式化输出
来源：http://duh.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ahs.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qyp.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mux.vqdsnc.cn

TS:   d.toISOString()
来源：http://upl.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lmc.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gvq.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pzn.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fqs.ivvv.top

[J03] 字符串解析为日期
来源：http://rsr.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kwk.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xdb.meibo888.top

JS:   new Date("2024-01-02")
来源：http://qxu.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://mzl.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://pvy.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sak.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://kcu.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fvi.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://ija.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sge.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gvt.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ysd.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ovl.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://agm.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kxn.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://usk.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cem.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://zbw.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://gzu.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fgc.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ink.yvedp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ehz.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://ffg.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eus.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://qvx.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://hlj.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://tlp.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://gth.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://owm.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mhp.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oqs.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lzs.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://onc.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://cav.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://zyf.sweek.top

[J07] 比较两个日期
来源：http://osj.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://dii.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wic.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xwt.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rdi.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sut.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ioa.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://hfo.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://pkv.yonumen.top

[J08] 提取年月日与星期
来源：http://psa.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uuz.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rte.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://edt.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xxt.shangyingyoupin.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://irq.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bfs.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cla.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://axj.xylfe.cn

[J09] 时区处理
来源：http://vhm.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jim.birdmap.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bky.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ksv.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ahz.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zfe.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dwg.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dim.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wct.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://xaf.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wrr.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hrc.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zut.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dbq.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jlb.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jhi.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rvk.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vsl.jinqigfzy.top

================================================================================
来源：http://apq.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://taj.jqgufenzy.top

================================================================================
来源：http://fhb.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://byq.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pnz.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lmw.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://jwo.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://xqk.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mlp.guannengcc.top

Go:   json.Marshal(obj)
来源：http://ndd.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cva.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vfq.ivvv.top

[K02] JSON 字符串转对象
来源：http://vub.0kj1m.cn

Py:   json.loads(s)
来源：http://dwi.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kub.tanke756.top

JS:   JSON.parse(s)
来源：http://zis.cucudq.cn

TS:   JSON.parse(s)
来源：http://awf.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mds.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://yrh.epnwcf.com

Ruby: JSON.parse(s)
来源：http://iqc.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vfr.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://jeh.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jui.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gsc.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yfu.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lwv.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://obt.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://glr.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://twd.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kai.shuidangran.top

[K04] 读取 JSON 文件
来源：http://xwd.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kix.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jku.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fzf.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ezi.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xrt.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aqo.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lso.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ofs.fehbvm.com

[K05] 深拷贝对象
来源：http://dhy.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://ali.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://nyf.zycfv.cn

JS:   structuredClone(obj)
来源：http://sqh.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://hnr.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fao.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oxy.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ven.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://joz.yj20258888.top

[K06] 解析 URL 查询串
来源：http://sbh.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tee.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wlp.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uau.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vmt.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gaf.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vor.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ogy.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tip.ehwqpu.com

[K07] 进制转换
来源：http://kls.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zmy.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ekm.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://afc.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://osm.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ydl.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tzz.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jqe.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qmh.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://cau.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://qpu.zhijiandao.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vbd.cqqwz.cn

JS:   v8.serialize(obj)        // Node
来源：http://jju.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://gne.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qvy.ehwqpu.com

Go:   encoding/gob
来源：http://ttw.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://bjo.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lne.guowangkeji.top

================================================================================
来源：http://ztk.vqdsnc.cn

L. 网络请求
来源：http://mbo.tianlin.xyz

================================================================================
来源：http://fuh.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://nwh.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://elo.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dtx.vqdsnc.cn

JS:   await fetch(url)
来源：http://cng.shzxlz.cn

TS:   await fetch(url)
来源：http://gpl.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://whk.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://sdz.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fwr.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lji.sufxvd.cn

[L02] 发送 POST JSON
来源：http://hks.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://ysx.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dts.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lki.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://obz.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rfp.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ydv.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://byz.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mnn.cucudq.cn

[L03] 设置自定义请求头
来源：http://isj.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xkg.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bam.jqgfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://siw.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vyb.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://axn.yangfankeji.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://akc.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rhg.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qqn.vqdsnc.cn

[L04] 设置超时
来源：http://zrf.tian-w.cn

Py:   requests.get(url, timeout=5)
来源：http://tzu.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jba.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xvi.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vet.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ous.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mvv.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oaa.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rkp.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://zys.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://axt.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lcv.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vpm.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bvr.gotoacloud.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bgn.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dyi.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://srg.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yxs.tian-w.cn

[L06] 解析响应为 JSON
来源：http://cxr.zdqjudy.top

Py:   resp.json()
来源：http://zyj.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://wvg.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://siy.iojbl.cn

TS:   await resp.json()
来源：http://zrt.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wiy.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dbo.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://zls.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://igw.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://xdc.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ros.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kru.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://vrj.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://org.jinqigufen.top

Java: resp.statusCode()
来源：http://yvq.uphjek.com

Go:   resp.StatusCode
来源：http://rpv.52xcode.cn

Ruby: resp.code.to_i
来源：http://knh.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://fgk.52xcode.cn

[L08] 并发请求多个地址
来源：http://wjf.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rxi.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://bju.jlsjyb.cn


<!-- 参考信息 -->