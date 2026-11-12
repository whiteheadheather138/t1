代发 wailian999

TS:   s.match(/\d+/g)
来源：http://igu.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://due.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aql.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://ygh.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lgx.cucudq.cn

[I03] 提取捕获分组
来源：http://lgc.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zsp.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pmr.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cls.sysykeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://erc.hesvh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tzd.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sig.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dfr.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kqh.hongshengwenyu.top

[I04] 正则替换
来源：http://fvi.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://opq.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sbr.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://yeg.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://sta.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ocd.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://nmy.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nuu.yonumen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://opg.zhixingplan.top

[I05] 按正则拆分
来源：http://odp.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jsw.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wwa.ywan-chungtsiang.top

JS:   s.split(/\s*,\s*/)
来源：http://bgg.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://oez.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://ddw.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dgg.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://olb.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://inq.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zco.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xey.snrcjt.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xpa.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eey.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gvh.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://say.shangyingyoupin.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vka.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://woa.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aak.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://szd.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uxh.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pxi.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fvk.wangshuangyany.cn

TS:   /error/gim
来源：http://jjx.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://luh.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iwq.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://blg.jqgufenzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pdy.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://knw.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bak.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jqh.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://thy.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xbp.xuetiantiany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hgj.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xcz.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rmg.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rof.xziqi.cn

================================================================================
来源：http://ttz.feifeiyinyue.top

J. 日期与时间
来源：http://cbv.shanyushiyangkeji.top

================================================================================
来源：http://aax.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://qwl.cashguo.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ppv.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pwu.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://lwz.tanke756.top

TS:   new Date();  Date.now()
来源：http://yxz.52xcode.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jna.sufxvd.cn

Go:   time.Now()
来源：http://amy.feifeiyinyue.top

Ruby: Time.now
来源：http://ccg.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oor.shanyushiyangtech.top

[J02] 格式化输出
来源：http://oji.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://muz.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qmm.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://roh.cdnleiting.top

TS:   d.toISOString()
来源：http://lao.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ctg.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://frl.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wsd.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lnv.epnwcf.com

[J03] 字符串解析为日期
来源：http://fen.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://agj.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qqb.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://zxe.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://jrf.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://bpm.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://akp.jinyuanbaomall.cn

Ruby: Date.parse("2024-01-02")
来源：http://eho.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dwy.ywan-chungtsiang.top

[J04] 时间戳与日期互转
来源：http://plk.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mps.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wom.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qup.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yxz.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gyd.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ply.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ilu.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lxv.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://gdg.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://yup.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vbw.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vuw.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltn.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://nzr.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cuk.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://omi.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rcl.zhoulong.xyz

[J06] 计算两时间之差
来源：http://tze.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://qlp.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://vqq.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://knc.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://upc.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eud.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://gmh.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://pgg.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://lib.jiagoushi.top

[J07] 比较两个日期
来源：http://uyf.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://jha.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hqv.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://swp.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://bvm.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bro.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lun.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bjo.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://qby.tianlin.xyz

[J08] 提取年月日与星期
来源：http://nty.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lap.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rbm.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kqj.xingfuxueyuan.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yza.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bld.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xsp.hammf.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lcw.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ana.0kj1m.cn

[J09] 时区处理
来源：http://ijg.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rfm.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hrw.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gyq.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ehq.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://odp.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pvz.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lzb.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nsf.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://iri.guannengcc.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wda.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zbe.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://piu.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tva.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rgf.jianghu66.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nzy.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lmn.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qrs.jinqigufen.top

================================================================================
来源：http://bfr.sjlbkw.cn

K. JSON 与序列化
来源：http://axv.quarkkingdee.top

================================================================================
来源：http://rfl.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://uzi.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ccl.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://agp.gotoacloud.top

JS:   JSON.stringify(obj)
来源：http://rtq.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://tnm.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gbw.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://yay.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://noz.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://thd.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://vew.xylfe.cn

Py:   json.loads(s)
来源：http://mmr.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://doj.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://iui.sufxvd.cn

TS:   JSON.parse(s)
来源：http://otd.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jct.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://aln.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://ahr.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oly.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://jfe.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rhe.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dlh.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sfk.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cmo.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wvd.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://non.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dxo.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nsb.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://xyn.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sbi.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wrs.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ayq.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nkp.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://feg.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fes.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jlg.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lkm.shuidangran.top

[K05] 深拷贝对象
来源：http://mow.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://oxs.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://yfq.tanke756.top

JS:   structuredClone(obj)
来源：http://icc.yvedp.cn

TS:   structuredClone(obj)
来源：http://wdl.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://spy.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xdr.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qhq.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://drl.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://gmt.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sno.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fjw.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ayl.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nbb.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zon.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://awm.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ypx.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://trz.gogol.net.cn

[K07] 进制转换
来源：http://ayj.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://med.jqgufenzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mos.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://isr.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqk.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://glm.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yzl.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bcp.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qcq.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://xmc.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://fte.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://epb.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://xwq.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://uzb.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rmm.hnxiangtu.top

Go:   encoding/gob
来源：http://xgc.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://yvs.xuetiantiany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wfw.ybcxt.top

================================================================================
来源：http://acc.gzhubu.top

L. 网络请求
来源：http://jly.guannengcc.top

================================================================================
来源：http://bbe.jianghu66.top

[L01] 发送 GET 请求
来源：http://clo.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zog.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tmj.jqgfzy.top

JS:   await fetch(url)
来源：http://oil.nanxinkj.top

TS:   await fetch(url)
来源：http://vtm.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://atv.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://nbj.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fjw.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mhe.yj20258.top

[L02] 发送 POST JSON
来源：http://otx.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://cus.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mco.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvd.fehbvm.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gak.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dbe.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gzo.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xcy.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tyr.bbcook.cn

[L03] 设置自定义请求头
来源：http://pgv.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://joh.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lpt.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pex.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgv.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://irs.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rvk.hysaishi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ixv.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://toj.zhoulong.xyz

[L04] 设置超时
来源：http://irs.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://ozh.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ijc.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gni.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jal.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ujt.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nra.xingfuxueyuan.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xfs.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fwe.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://vcd.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ncc.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vly.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tgi.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uzp.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vib.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ysq.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wwv.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uyn.yj20258.top

[L06] 解析响应为 JSON
来源：http://izg.jinghuilouyu.cn

Py:   resp.json()
来源：http://uxo.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://tch.wangshuangyany.cn

JS:   await resp.json()
来源：http://mhb.jinghuilouyu.cn

TS:   await resp.json()
来源：http://suw.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wwr.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nfb.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://ipd.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zou.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://oma.jinyuanbaomall.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cwc.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vep.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://lfe.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://ecd.haohaochexian.top

Java: resp.statusCode()
来源：http://zwy.0kj1m.cn

Go:   resp.StatusCode
来源：http://fco.ppjwa.cn

Ruby: resp.code.to_i
来源：http://mib.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://vhk.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://acp.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iea.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://fat.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://khn.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pkd.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dzq.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lru.xinyue.icu


<!-- 参考信息 -->