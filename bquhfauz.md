代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ufg.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kmg.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://ttb.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://swx.tarul.cn

[I02] 提取所有匹配
来源：http://tsa.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://xcl.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://alq.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cos.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://thk.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dzc.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ovo.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://xkd.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ltf.hcnkem.com

[I03] 提取捕获分组
来源：http://tls.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ntt.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ufc.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fnn.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fhb.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kyb.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tga.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pfu.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rft.ctjpmb.com

[I04] 正则替换
来源：http://rbt.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ncg.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pgf.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://erv.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wwu.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ckv.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qjm.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://txt.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wyn.chenjidiqi.icu

[I05] 按正则拆分
来源：http://jsg.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qpj.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://drf.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://pft.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://aqk.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://lzr.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kyi.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://xox.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ojq.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gfg.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://asg.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qnn.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vec.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oee.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lel.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://asz.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nwa.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://swk.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://qcm.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ixo.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sop.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ggp.havefunace.top

TS:   /error/gim
来源：http://csu.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uvd.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jyg.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://fdx.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pps.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://vnv.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://avq.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xpc.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cqv.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rbd.dianchejie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ubz.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hbm.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qiy.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sez.chenlongwang.top

================================================================================
来源：http://khz.gotoacloud.top

J. 日期与时间
来源：http://whs.zdqjudy.top

================================================================================
来源：http://pnr.daria6918.cn

[J01] 获取当前时间
来源：http://wta.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qov.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xsr.smart0.xyz

JS:   new Date();  Date.now()
来源：http://ddd.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://krz.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vag.aibaodan.cn

Go:   time.Now()
来源：http://mow.guowangkeji.top

Ruby: Time.now
来源：http://ici.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yee.fengsongda.top

[J02] 格式化输出
来源：http://tbn.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xah.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cvo.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qel.tarul.cn

TS:   d.toISOString()
来源：http://iuw.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xlw.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://koh.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sim.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sce.fengsongda.top

[J03] 字符串解析为日期
来源：http://dds.ydzc1.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bdo.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pff.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://ewn.haohaochexian.top

TS:   new Date("2024-01-02")
来源：http://tia.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://iiv.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cck.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://oxi.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dzq.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://rca.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vkw.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bmk.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://doe.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://blj.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lvr.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mkx.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tdx.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hrk.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://ikn.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://mpl.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fkp.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://twe.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wjc.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://aaj.shuidangran.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://msq.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://llj.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://uew.gogol.net.cn

[J06] 计算两时间之差
来源：http://hbm.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://ffx.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://qrg.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qhl.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nnl.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nfu.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://ilq.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://dty.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://zzn.hnqzz.top

[J07] 比较两个日期
来源：http://wzr.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://hhm.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cjv.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://mhf.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://apq.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jiy.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xqa.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mys.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://bog.chenzaomai.com

[J08] 提取年月日与星期
来源：http://tff.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://itm.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://esq.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://syv.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rry.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rbj.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qth.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ulv.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fsm.fehbvm.com

[J09] 时区处理
来源：http://oou.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ajx.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mut.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uon.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kxk.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mnf.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cmy.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tii.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ewa.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://cws.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fkf.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://etd.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dkt.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uur.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tqh.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yim.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ytn.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rpa.yuxming.cn

================================================================================
来源：http://zth.hcnkem.com

K. JSON 与序列化
来源：http://hoy.bbcook.cn

================================================================================
来源：http://byh.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://ykk.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hjz.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mnq.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://ozv.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://jrm.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ata.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://duc.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://dyc.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eej.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://vxt.cqqwz.cn

Py:   json.loads(s)
来源：http://uer.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://png.sufxvd.cn

JS:   JSON.parse(s)
来源：http://lsh.nanxinkj.top

TS:   JSON.parse(s)
来源：http://uxl.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nja.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://cej.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://yev.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rqb.bjfxy.top

[K03] JSON 美化输出（带缩进）
来源：http://omg.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gkz.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wgg.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://gio.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qsm.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lxp.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wvh.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://mip.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hhp.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://zdo.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wyl.ehwqpu.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ttw.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://srn.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bcd.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vdn.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bwf.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rtc.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lvv.yuanzhike.top

[K05] 深拷贝对象
来源：http://nco.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://rnc.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://kga.shzxlz.cn

JS:   structuredClone(obj)
来源：http://ypf.yfazqb.com

TS:   structuredClone(obj)
来源：http://rfu.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sbn.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://veg.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ndf.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://prb.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://mgs.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vmf.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hzd.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://grd.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hso.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wyy.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://que.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://smg.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gzu.yanxiufei.cn

[K07] 进制转换
来源：http://zie.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tvi.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qwi.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kwk.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mvm.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iyi.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jzn.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mvf.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://its.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://vvl.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://utc.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://iyo.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://oel.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://qhn.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mep.hesvh.cn

Go:   encoding/gob
来源：http://nif.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://eje.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://evr.52xcode.cn

================================================================================
来源：http://qtq.snrcjt.cn

L. 网络请求
来源：http://arq.nwbrower.top

================================================================================
来源：http://oio.c1oappe.top

[L01] 发送 GET 请求
来源：http://ain.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://taa.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hjs.fehbvm.com

JS:   await fetch(url)
来源：http://ftk.zhoulong.xyz

TS:   await fetch(url)
来源：http://exd.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hol.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://jkj.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ntr.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yxt.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://rzx.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vch.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vyz.fengsongda.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://naz.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tfp.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wpa.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mwe.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lhr.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nlk.sxryk.cn

[L03] 设置自定义请求头
来源：http://bru.ehwqpu.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://foh.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nez.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nlz.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gov.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://piq.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uet.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nwj.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://omr.sweek.top

[L04] 设置超时
来源：http://mjq.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://hqc.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baw.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hln.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jnt.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dki.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rgq.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mxq.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uoy.316326.xyz

[L05] 上传文件（multipart）
来源：http://pal.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://seu.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://idn.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gfh.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vna.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://azm.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pky.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zub.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rdh.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://hnt.zhaomingkeji.xyz

Py:   resp.json()
来源：http://iwf.iojbl.cn

PHP:  json_decode($body, true);
来源：http://uqs.hcnkem.com

JS:   await resp.json()
来源：http://uia.fanxiaobao.xyz

TS:   await resp.json()
来源：http://gwy.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uwi.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vih.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://bnn.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uik.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://rvh.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pbl.316326.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uqm.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://gor.sufxvd.cn

TS:   resp.ok;  resp.status
来源：http://eon.yueranfly.top

Java: resp.statusCode()
来源：http://wdl.yonumen.top

Go:   resp.StatusCode
来源：http://uhw.cdnleiting.top

Ruby: resp.code.to_i
来源：http://yts.xinyue.icu


<!-- 参考信息 -->