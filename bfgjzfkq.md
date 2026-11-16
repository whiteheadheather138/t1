代发 wailian999

TS:   s.match(/\d+/g)
来源：http://vdi.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uce.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kpg.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://mok.hnqzz.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zsy.fktsv.cn

[I03] 提取捕获分组
来源：http://dcs.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uiq.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hnt.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bkn.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vxe.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://axz.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ded.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xfd.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yiy.hnqzz.top

[I04] 正则替换
来源：http://xmb.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zrm.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lan.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://mhd.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mem.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://wte.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://wmt.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hae.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nlh.guannengcc.top

[I05] 按正则拆分
来源：http://lpe.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://toi.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xjv.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://css.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://zgh.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://xii.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ari.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://tbc.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ajj.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jld.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jgz.kuanghao11.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xyw.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fbn.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pna.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://roo.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nmr.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pdy.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://afc.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://yyt.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zql.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xdo.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://flq.pycfn.com

TS:   /error/gim
来源：http://xwq.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vhr.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ksa.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://xer.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mqn.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://nbv.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wsx.redwolf501.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ozs.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xgw.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vwv.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uic.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ond.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jwq.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://opf.andypj.xyz

================================================================================
来源：http://htc.shanyushiyangtech.top

J. 日期与时间
来源：http://tbx.gzhubu.top

================================================================================
来源：http://ofj.tianlin.xyz

[J01] 获取当前时间
来源：http://lbg.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mxv.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rmt.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://gwc.aizwys.cn

TS:   new Date();  Date.now()
来源：http://lhv.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cxc.gaohongyu789.top

Go:   time.Now()
来源：http://nrp.fanxiaobao.xyz

Ruby: Time.now
来源：http://nrv.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://moc.shangyingyoupin.top

[J02] 格式化输出
来源：http://ryj.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tyn.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ezn.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bjj.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://wwi.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dvj.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bzl.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rdq.cucudq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://crr.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://lil.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://urk.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://voq.tarul.cn

JS:   new Date("2024-01-02")
来源：http://vgz.tanke756.top

TS:   new Date("2024-01-02")
来源：http://mlc.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://ock.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ikr.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://fsf.hnqzz.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://trb.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://diq.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://euo.zdbjq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://snr.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zwo.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ywp.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tkq.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://siq.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qgo.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ujd.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://afz.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://gym.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jbj.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fag.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kjn.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://kjd.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lxz.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://pik.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://jss.jlsjyb.cn

[J06] 计算两时间之差
来源：http://led.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://ahr.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://jga.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://flf.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mso.kuanghao11.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tgf.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://olh.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://noq.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://enb.zhiwuduotai.top

[J07] 比较两个日期
来源：http://efh.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://oku.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zud.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kuy.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://vjp.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bae.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wfp.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://xvp.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://zme.aizwys.cn

[J08] 提取年月日与星期
来源：http://trh.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wbt.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mcb.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wzy.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rat.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gfs.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jch.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ghp.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hmo.guannengcc.top

[J09] 时区处理
来源：http://ygj.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wlm.xylfe.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lin.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xoz.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qar.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pzp.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lce.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ihn.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://igd.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://hxr.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://far.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qyr.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hyw.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gln.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qdg.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ndp.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ksc.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://esg.andypj.xyz

================================================================================
来源：http://uxk.cashguo.top

K. JSON 与序列化
来源：http://oaw.wangshuangyany.cn

================================================================================
来源：http://psd.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://ips.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ezd.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xkh.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://hwl.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://ydh.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jrc.pycfn.com

Go:   json.Marshal(obj)
来源：http://kot.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://xis.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vsr.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://tpj.jlsjyb.cn

Py:   json.loads(s)
来源：http://ras.shangyingyoupin.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xol.hammf.cn

JS:   JSON.parse(s)
来源：http://ypr.tianlin.xyz

TS:   JSON.parse(s)
来源：http://yme.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cct.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://qkq.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://ihm.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mdf.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://jpt.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yby.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ffa.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sep.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cys.hongshengwenyu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qyi.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xlk.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://fza.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://daz.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://oxx.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cvp.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fvj.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mfy.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rsn.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://usw.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ihs.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yie.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yng.smart0.xyz

[K05] 深拷贝对象
来源：http://mkt.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://drn.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://ypw.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://wln.cqqwz.cn

TS:   structuredClone(obj)
来源：http://qcs.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xwn.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mta.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ihy.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qzw.yfazqb.com

[K06] 解析 URL 查询串
来源：http://whc.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cyl.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vlz.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jqm.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wao.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fsh.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rra.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sms.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tel.bbcook.cn

[K07] 进制转换
来源：http://fyr.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cne.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ned.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vtl.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ytw.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kjo.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wox.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ako.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ibu.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://ovx.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://oxy.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bes.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://stw.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://cbw.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wwx.tianlin.xyz

Go:   encoding/gob
来源：http://yaz.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://iqt.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cnf.zhongyouzk.top

================================================================================
来源：http://ekc.cashguo.top

L. 网络请求
来源：http://ysk.ydjk.org.cn

================================================================================
来源：http://nbp.chenzaomai.com

[L01] 发送 GET 请求
来源：http://ciq.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wwg.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hxw.vehdjk.com

JS:   await fetch(url)
来源：http://ora.yfazqb.com

TS:   await fetch(url)
来源：http://tln.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jra.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://ayz.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zzu.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fsu.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://tpj.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://all.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xxx.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zkx.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fxe.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://arb.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jvg.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dif.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bwq.ehwqpu.com

[L03] 设置自定义请求头
来源：http://vvh.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://htx.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xwj.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vif.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bmx.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lvr.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mtv.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aiv.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ibe.yfazqb.com

[L04] 设置超时
来源：http://pbr.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://erm.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://skc.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ioy.ydzc1.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jbl.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://owf.sufxvd.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://epa.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gpt.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://net.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://cdx.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://leu.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rif.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://img.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kpn.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sel.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://caw.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lzx.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zor.ydzc1.top

[L06] 解析响应为 JSON
来源：http://tbm.bjfxy.top

Py:   resp.json()
来源：http://hxq.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://rso.nwbrower.top

JS:   await resp.json()
来源：http://fih.dashuyun.cn

TS:   await resp.json()
来源：http://msx.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zbx.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wsu.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://bca.ehwqpu.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bcj.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://wzd.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yye.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://icd.cheryme.top

JS:   resp.ok;  resp.status
来源：http://usa.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://lhj.bjfxy.top

Java: resp.statusCode()
来源：http://ugs.sjlbkw.cn

Go:   resp.StatusCode
来源：http://izk.xuanzx.com

Ruby: resp.code.to_i
来源：http://liv.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://frt.shuidangran.top

[L08] 并发请求多个地址
来源：http://emk.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pnu.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://lcm.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rhl.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bss.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zur.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://doi.yfazqb.com


<!-- 参考信息 -->