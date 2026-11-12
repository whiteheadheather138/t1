代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jme.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://klj.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://esd.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zej.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vgi.hnqzz.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ryk.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://anm.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xbe.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vkn.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mdf.havefunace.top

[I04] 正则替换
来源：http://hbt.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ahd.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://npd.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kbg.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://bvl.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://nps.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dbl.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gbh.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iga.guowangkeji.top

[I05] 按正则拆分
来源：http://siw.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xmf.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://opg.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://xym.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://bsh.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://yna.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qvp.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://baz.yueranfly.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hib.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eho.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uqa.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rpd.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eue.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://orn.hnxiangtu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hso.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blm.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eud.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jid.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://bcg.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qfy.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mis.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sqm.pengpengdd.cyou

TS:   /error/gim
来源：http://feb.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rqi.daxiang520.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pdn.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://kyf.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gru.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://jfk.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zqt.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bvu.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ybg.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rnz.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uac.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qas.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uhr.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://idn.shangyingyoupin.top

================================================================================
来源：http://gkc.ybcxt.top

J. 日期与时间
来源：http://adh.snrcjt.cn

================================================================================
来源：http://jlw.wangdashe.top

[J01] 获取当前时间
来源：http://dxo.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wbz.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fav.cheryme.top

JS:   new Date();  Date.now()
来源：http://dco.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://oau.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hvm.pengpengdd.cyou

Go:   time.Now()
来源：http://cxw.hysaishi.cn

Ruby: Time.now
来源：http://rmm.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blb.shanyushiyangtech.top

[J02] 格式化输出
来源：http://kuy.jqgufenzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://swl.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://imw.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gzq.0kj1m.cn

TS:   d.toISOString()
来源：http://lxe.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hma.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xik.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rcn.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xsd.gotoacloud.top

[J03] 字符串解析为日期
来源：http://esc.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hyg.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kab.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://byh.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://ufy.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sai.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cib.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://zoy.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hfl.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://bno.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lhe.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://khx.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zsn.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ljb.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hoz.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tgu.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wzj.yj20258888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://idh.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://lup.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://vnu.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zsf.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nwm.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://icw.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://wqn.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kxl.quarkkingdee.top

Ruby: Time.now + 7 * 86400
来源：http://fsj.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rtq.yuanzhike.top

[J06] 计算两时间之差
来源：http://fvs.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://llv.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://twa.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eny.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://feq.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://oox.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://aue.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://wky.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://axc.cheryme.top

[J07] 比较两个日期
来源：http://pay.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://zzc.andypj.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gew.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://pjx.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ldo.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://flm.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fyt.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://rjw.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://jfn.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://jai.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tfq.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zjt.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nxw.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pyb.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://obn.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lpr.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nan.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tgk.chenzaomai.com

[J09] 时区处理
来源：http://ggm.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fep.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qcu.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hsx.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://krx.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sek.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://map.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dhg.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qul.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://rpa.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://qbj.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iil.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iub.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fto.bjfxy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://coh.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qgs.52xcode.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rrv.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iyz.shzxlz.cn

================================================================================
来源：http://yvr.wangshuangyany.cn

K. JSON 与序列化
来源：http://zeh.yj202588.top

================================================================================
来源：http://owf.hfpthk.cn

[K01] 对象转 JSON 字符串
来源：http://fbo.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nqz.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zmr.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://mmw.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://urf.zhiwuduotai.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gio.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://qoa.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://axm.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vdb.daxiang520.top

[K02] JSON 字符串转对象
来源：http://sqc.meibo888.top

Py:   json.loads(s)
来源：http://ynw.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ctz.yuanzhike.top

JS:   JSON.parse(s)
来源：http://vmd.cheryme.top

TS:   JSON.parse(s)
来源：http://oio.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ows.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://pjl.tarul.cn

Ruby: JSON.parse(s)
来源：http://lak.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bjh.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://zjw.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rtn.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jst.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vaj.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mvt.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rzk.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wcq.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://ouz.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hbu.jianghu66.top

[K04] 读取 JSON 文件
来源：http://hvg.xuanzx.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jxa.yj20258.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ues.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://euc.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pjr.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dyw.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lps.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ars.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xoy.iojbl.cn

[K05] 深拷贝对象
来源：http://ids.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://bon.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://oil.jiagoushi.top

JS:   structuredClone(obj)
来源：http://cmk.ehwqpu.com

TS:   structuredClone(obj)
来源：http://nzn.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://xrm.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ief.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cxa.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oxh.sxryk.cn

[K06] 解析 URL 查询串
来源：http://btj.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jnp.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ial.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vau.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wyn.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eok.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rjn.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mwn.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mai.zhoulong.xyz

[K07] 进制转换
来源：http://xkw.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nbk.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://obd.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vta.wangshuangyany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cuk.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hwq.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rza.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xho.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://she.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://sam.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://gwe.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rqi.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://lmo.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://yuc.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ihl.nwbrower.top

Go:   encoding/gob
来源：http://slp.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://ffs.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jrg.xinyue.icu

================================================================================
来源：http://ien.yj20258888.top

L. 网络请求
来源：http://ynv.ivvv.top

================================================================================
来源：http://hqv.jianghu66.top

[L01] 发送 GET 请求
来源：http://wzn.shanyushiyangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mbp.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dbu.yueranfly.top

JS:   await fetch(url)
来源：http://kfu.zhixingplan.top

TS:   await fetch(url)
来源：http://kpl.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lbq.vehdjk.com

Go:   resp, err := http.Get(url)
来源：http://fev.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eye.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xcf.yangfankeji.com

[L02] 发送 POST JSON
来源：http://wnw.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://pfx.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hgz.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lic.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://muu.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iod.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vrb.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lfc.hysaishi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ayf.sweek.top

[L03] 设置自定义请求头
来源：http://dii.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xuz.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wrl.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jkz.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vft.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gbh.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yyg.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xql.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://boh.xuanzx.com

[L04] 设置超时
来源：http://nqy.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://kip.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ozb.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://woz.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oqn.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iid.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tnf.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ncw.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lze.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://rpt.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mrx.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://njc.yongpay.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://icj.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ztl.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://loa.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rzd.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rcg.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://she.yj202588.top

[L06] 解析响应为 JSON
来源：http://ojt.sysykeji.top

Py:   resp.json()
来源：http://poc.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://iwf.sjlbkw.cn

JS:   await resp.json()
来源：http://uif.nanxinkj.top

TS:   await resp.json()
来源：http://mog.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://snu.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wfo.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://eal.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oxj.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://xyc.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hkq.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ggn.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://qfw.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://kxy.gaohongyu789.top

Java: resp.statusCode()
来源：http://bqs.zhongyouzk.top

Go:   resp.StatusCode
来源：http://ira.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://xvl.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://yhr.xinyue.icu

[L08] 并发请求多个地址
来源：http://tto.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zbt.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://zhp.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wrf.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qht.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oes.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hcr.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tsu.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iwg.daxiang520.top

================================================================================
来源：http://kod.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://njp.shuidangran.top


<!-- 参考信息 -->