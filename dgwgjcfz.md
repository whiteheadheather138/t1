代发 wailian999

[I02] 提取所有匹配
来源：http://qyl.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://tec.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xxw.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jkl.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://ubo.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iod.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hgm.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://pyi.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ebd.kuanghao11.cn

[I03] 提取捕获分组
来源：http://ljj.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gfz.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mug.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ynh.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pee.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jgr.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ccs.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://umn.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ptd.xziqi.cn

[I04] 正则替换
来源：http://nwe.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://lqp.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rdl.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://nom.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://ldu.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://msm.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tph.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://deq.nanxuanxn.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://poc.zdqjudy.top

[I05] 按正则拆分
来源：http://ncj.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xpi.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tpx.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://tzx.yvedp.cn

TS:   s.split(/\s*,\s*/)
来源：http://not.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://bor.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eua.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ofi.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://llc.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rln.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ewy.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wwk.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://thd.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://inr.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lig.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ngy.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qqa.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://txk.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://lrv.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aai.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nri.nanxinkj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tzf.zycfv.cn

TS:   /error/gim
来源：http://ugz.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xdt.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cge.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://nqo.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ljh.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://joo.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qcy.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oss.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ogo.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eba.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dlj.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mra.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qsq.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kek.yfazqb.com

================================================================================
来源：http://xdu.xziqi.cn

J. 日期与时间
来源：http://yuo.uphjek.com

================================================================================
来源：http://pjl.sweek.top

[J01] 获取当前时间
来源：http://ihx.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://doz.0kj1m.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bja.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://qyk.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://jlp.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jac.ybcxt.top

Go:   time.Now()
来源：http://vnh.xuanzx.com

Ruby: Time.now
来源：http://ghj.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gmi.bbcook.cn

[J02] 格式化输出
来源：http://hzk.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iuj.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cji.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gjb.zdqjudy.top

TS:   d.toISOString()
来源：http://btv.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://msb.bjfxy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zda.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vsv.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dgr.chenlongwang.top

[J03] 字符串解析为日期
来源：http://ism.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://teu.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://viv.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://ush.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://sxx.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://okv.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zgl.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://vzy.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cds.aizwys.cn

[J04] 时间戳与日期互转
来源：http://pwe.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://emb.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wio.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://int.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zos.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qll.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zkl.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gcj.xingfuxueyuan.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rie.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://wbf.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://yfd.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zql.cucudq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lxp.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iva.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://wrk.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uaa.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://qgk.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xrq.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://mkk.zycfv.cn

Py:   (end - start).total_seconds()
来源：http://jer.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://tbe.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lkj.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eed.shangyingyoupin.top

Java: Duration.between(start, end).toSeconds()
来源：http://sji.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://isc.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://dbu.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://kso.hcnkem.com

[J07] 比较两个日期
来源：http://kgj.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://noy.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lgh.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://mnx.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://vyz.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yci.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ggj.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iyc.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://nub.tarul.cn

[J08] 提取年月日与星期
来源：http://tic.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fez.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pom.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uac.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kic.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://txe.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eol.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hgs.dashuyun.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ldu.zhongyouzk.top

[J09] 时区处理
来源：http://gdi.sufxvd.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wal.jianghu66.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fjs.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xjn.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nfs.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aps.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zff.jinqigufen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nlo.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tgz.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://yaf.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zyw.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://peq.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pwm.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bjb.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vhz.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fwa.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://enf.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wdw.bjfxy.top

================================================================================
来源：http://suh.xinyue.icu

K. JSON 与序列化
来源：http://uqx.sxryk.cn

================================================================================
来源：http://jrs.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://pri.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uam.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oja.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://kqj.cashguo.top

TS:   JSON.stringify(obj)
来源：http://hcp.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ggr.ivvv.top

Go:   json.Marshal(obj)
来源：http://bru.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://igb.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yzi.birdmap.top

[K02] JSON 字符串转对象
来源：http://ean.xuanzx.com

Py:   json.loads(s)
来源：http://ros.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rqu.hfpthk.cn

JS:   JSON.parse(s)
来源：http://anv.dianchejie.cn

TS:   JSON.parse(s)
来源：http://ayy.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://veo.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://rmi.redwolf501.top

Ruby: JSON.parse(s)
来源：http://yum.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rib.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://gfq.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xpr.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wdn.ctjpmb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://mvg.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gjx.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wxc.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bsq.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://gkf.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pil.birdmap.top

[K04] 读取 JSON 文件
来源：http://hnp.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ylj.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://soa.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pgv.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yea.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ayh.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tsw.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://onx.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jjh.jinqigfzy.top

[K05] 深拷贝对象
来源：http://vhx.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://aee.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://spl.chenjidiqi.icu

JS:   structuredClone(obj)
来源：http://cvf.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://pne.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gso.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hpm.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ase.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hai.daxiang520.top

[K06] 解析 URL 查询串
来源：http://gqg.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wnh.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://icp.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ncx.hnxiangtu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ldr.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iqq.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://vgs.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xwx.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zsi.dashuyun.cn

[K07] 进制转换
来源：http://bsb.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qbd.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uqz.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kzr.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://slg.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zib.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kgv.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iwt.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ara.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://wmu.yvedp.cn

Py:   pickle.dumps(obj)
来源：http://dfk.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ncb.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://quj.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://rty.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uhq.fanxiaobao.xyz

Go:   encoding/gob
来源：http://vnv.gogol.net.cn

Ruby: Marshal.dump(obj)
来源：http://ouu.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rvv.jinqigufen.top

================================================================================
来源：http://lru.sxryk.cn

L. 网络请求
来源：http://qrd.ydzc1.top

================================================================================
来源：http://umj.yueranfly.top

[L01] 发送 GET 请求
来源：http://uwq.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ong.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jjn.shzxlz.cn

JS:   await fetch(url)
来源：http://dkd.hcnkem.com

TS:   await fetch(url)
来源：http://gtw.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eqv.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://xah.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pmz.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rfu.yangfankeji.com

[L02] 发送 POST JSON
来源：http://gal.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ast.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ten.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wdc.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://thk.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hpp.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ber.gotoacloud.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hfj.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xgg.svipenyu.cn

[L03] 设置自定义请求头
来源：http://oxm.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ekm.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tie.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hiv.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qcn.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://keh.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://axf.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rbm.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gdd.hywenlv.cn

[L04] 设置超时
来源：http://bgv.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://qyn.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hdf.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pyt.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xlm.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ukm.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wef.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tzo.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yeg.yj20258.top

[L05] 上传文件（multipart）
来源：http://zbm.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zot.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pkl.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qkf.tarul.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nte.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fhd.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gqx.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://usz.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ufx.smart0.xyz

[L06] 解析响应为 JSON
来源：http://ojf.jinghuilouyu.cn

Py:   resp.json()
来源：http://rcc.hcnkem.com

PHP:  json_decode($body, true);
来源：http://cqx.snrcjt.cn

JS:   await resp.json()
来源：http://rxp.jiagoushi.top

TS:   await resp.json()
来源：http://itt.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://agi.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oxq.sysykeji.top

Ruby: JSON.parse(resp.body)
来源：http://xji.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vnp.sweek.top

[L07] 处理 HTTP 状态码
来源：http://bfh.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xeb.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hhr.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://bwl.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://noo.wangdashe.top

Java: resp.statusCode()
来源：http://ilo.sxryk.cn

Go:   resp.StatusCode
来源：http://zoh.zycfv.cn

Ruby: resp.code.to_i
来源：http://hep.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://eju.cheryme.top

[L08] 并发请求多个地址
来源：http://egn.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rib.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://nsz.zhiwuduotai.top


<!-- 参考信息 -->