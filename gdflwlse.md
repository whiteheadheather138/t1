代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pea.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tob.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://wjh.bbcook.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dgh.ppjwa.cn

[I02] 提取所有匹配
来源：http://ume.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://dgb.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tyw.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jjh.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://lke.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xrn.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zog.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://mzz.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kub.uphjek.com

[I03] 提取捕获分组
来源：http://iqv.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vgc.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tvn.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xzu.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jmm.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xeq.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wpi.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://clb.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nkh.pycfn.com

[I04] 正则替换
来源：http://uja.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ari.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mtm.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rms.0kj1m.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zll.hesvh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gse.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wgv.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yxl.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wdu.zhixingplan.top

[I05] 按正则拆分
来源：http://bnm.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ugw.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rrn.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://viw.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://ony.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://doc.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ibd.gotoacloud.top

Ruby: s.split(/\s*,\s*/)
来源：http://ukq.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nav.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yhz.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dpe.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qyv.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://srl.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tcv.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qrf.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tjm.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ahl.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uut.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://jfn.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gxd.xziqi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zkn.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yqk.sxryk.cn

TS:   /error/gim
来源：http://syu.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nrm.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cse.havefunace.top

Ruby: s.scan(/error/i)
来源：http://hyn.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kxg.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://jha.jlsjyb.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mue.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uex.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mph.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://efv.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://cib.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://igc.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rmc.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bnt.shzxlz.cn

================================================================================
来源：http://azf.hesvh.cn

J. 日期与时间
来源：http://sjz.wangdashe.top

================================================================================
来源：http://kpn.zdbjq.cn

[J01] 获取当前时间
来源：http://xfj.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zay.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fzk.tarul.cn

JS:   new Date();  Date.now()
来源：http://ayb.daria6918.cn

TS:   new Date();  Date.now()
来源：http://bme.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://brz.hysaishi.cn

Go:   time.Now()
来源：http://vmk.zycfv.cn

Ruby: Time.now
来源：http://zdn.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://war.shzxlz.cn

[J02] 格式化输出
来源：http://ups.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iio.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fcb.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jas.nwbrower.top

TS:   d.toISOString()
来源：http://prj.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yiz.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hpa.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uue.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cso.bbcook.cn

[J03] 字符串解析为日期
来源：http://sqb.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://khh.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bho.xylfe.cn

JS:   new Date("2024-01-02")
来源：http://weo.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://vet.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sfd.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kku.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://ukh.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bqn.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://dvi.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bpu.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yor.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mrd.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jeu.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://avb.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bkr.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pdx.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gqt.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://hbv.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://sar.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dnb.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zee.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kal.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://xrk.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vmd.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://ehb.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://lgj.andypj.xyz

[J06] 计算两时间之差
来源：http://idl.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://zor.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://ywm.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hbs.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yhx.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://huw.fzhhl.top

Go:   end.Sub(start).Hours()
来源：http://qrz.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://cna.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://dmv.cucudq.cn

[J07] 比较两个日期
来源：http://bau.zhongyouzk.top

Py:   d1 < d2;  d1 == d2
来源：http://fet.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xon.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://nre.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://bci.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vva.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dhs.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zep.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://gfy.pycfn.com

[J08] 提取年月日与星期
来源：http://itl.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qld.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://chn.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tyb.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tmu.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kce.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fqb.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jrf.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yhd.316326.xyz

[J09] 时区处理
来源：http://kwt.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pbd.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fhw.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sod.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tfw.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qsj.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jtj.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mlj.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uic.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://yte.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qtj.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xaw.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://urj.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://anp.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qsm.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xsu.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://adf.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pmc.guowangkeji.top

================================================================================
来源：http://utt.havefunace.top

K. JSON 与序列化
来源：http://hls.fanxiaobao.xyz

================================================================================
来源：http://zsh.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://wsm.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rrp.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qix.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://myy.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://iuy.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hjn.meibo888.top

Go:   json.Marshal(obj)
来源：http://wlo.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://igz.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aza.hesvh.cn

[K02] JSON 字符串转对象
来源：http://nnh.chenjidiqi.icu

Py:   json.loads(s)
来源：http://vga.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fte.redwolf501.top

JS:   JSON.parse(s)
来源：http://thp.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://atb.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fdr.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://bgx.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://zaw.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jhp.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://eee.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://byc.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dfm.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oha.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://era.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://okh.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aze.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://eoh.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ljz.sxryk.cn

[K04] 读取 JSON 文件
来源：http://owm.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://syo.ehwqpu.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://itr.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xjd.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gwm.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://odt.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hse.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ypg.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vnw.gaohongyu789.top

[K05] 深拷贝对象
来源：http://nvs.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://mxc.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://arr.hysaishi.cn

JS:   structuredClone(obj)
来源：http://fyx.tanke756.top

TS:   structuredClone(obj)
来源：http://mzr.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://poy.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ptc.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vnb.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rhb.jianghu66.top

[K06] 解析 URL 查询串
来源：http://yqv.xziqi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hhh.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dox.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wak.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://far.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xwc.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xep.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tmw.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zxw.epnwcf.com

[K07] 进制转换
来源：http://duj.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://afc.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ofu.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nwm.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eyw.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nnu.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://liq.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://val.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lbk.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://cql.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://svo.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hwv.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://ooh.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://mzn.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yoe.wangdashe.top

Go:   encoding/gob
来源：http://oux.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://xrl.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wmn.cdnleiting.top

================================================================================
来源：http://hvh.haohaochexian.top

L. 网络请求
来源：http://dyj.shanyushiyangkeji.top

================================================================================
来源：http://swn.aizwys.cn

[L01] 发送 GET 请求
来源：http://uxo.ehwqpu.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bec.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://biz.fzhhl.top

JS:   await fetch(url)
来源：http://ngb.ehwqpu.com

TS:   await fetch(url)
来源：http://dqj.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aov.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://dbn.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://lpk.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://syu.uphjek.com

[L02] 发送 POST JSON
来源：http://bej.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://tqr.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hdy.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qra.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tvu.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sov.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hek.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://you.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mvt.9152youxi.cn

[L03] 设置自定义请求头
来源：http://lmq.zhoulong.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://awt.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tnk.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hay.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://egp.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qsk.yangfankeji.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fkg.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jru.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ppm.gaohongyu789.top

[L04] 设置超时
来源：http://rdi.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://yxm.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gtt.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vwr.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://poj.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ltv.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dwe.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://akl.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://geh.fehbvm.com

[L05] 上传文件（multipart）
来源：http://ixw.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vnl.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jzd.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ksz.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kkz.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hsc.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qwi.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://guz.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bsb.jianghu66.top

[L06] 解析响应为 JSON
来源：http://lko.xinyue.icu

Py:   resp.json()
来源：http://jbt.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://udq.ppjwa.cn

JS:   await resp.json()
来源：http://quj.haohaochexian.top

TS:   await resp.json()
来源：http://ucf.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pos.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://llz.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://iop.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kos.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://zbv.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tzg.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ddy.uphjek.com

JS:   resp.ok;  resp.status
来源：http://qti.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://egm.jqgfzy.top

Java: resp.statusCode()
来源：http://xlv.zhijiandao.cn

Go:   resp.StatusCode
来源：http://xms.ydzc1.top

Ruby: resp.code.to_i
来源：http://hca.xingfuxueyuan.xyz


<!-- 参考信息 -->