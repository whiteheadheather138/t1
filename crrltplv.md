代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ali.xuetiantiany.cn

[I03] 提取捕获分组
来源：http://kwb.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gyb.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rmk.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hjc.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zob.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cin.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://znj.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dpk.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ujm.yj20258.top

[I04] 正则替换
来源：http://kpt.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://myx.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hey.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://myy.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qrf.aibaodan.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ckd.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://htw.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://zeb.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dvu.yongpay.top

[I05] 按正则拆分
来源：http://pjg.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://suz.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ofg.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://xej.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://wwi.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://tnu.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sqq.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://tfl.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hkx.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qkq.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://llx.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kua.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://saq.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wpr.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://raw.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ise.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://upg.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kss.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://deh.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xyi.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uwf.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wcn.xylfe.cn

TS:   /error/gim
来源：http://myd.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://umt.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ofb.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://fpi.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rmj.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://ell.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pzn.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uce.birdmap.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lay.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://reh.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://spt.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wsu.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://udu.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dtp.xuanzx.com

================================================================================
来源：http://nnf.jlsjyb.cn

J. 日期与时间
来源：http://ews.hfpthk.cn

================================================================================
来源：http://ktz.hammf.cn

[J01] 获取当前时间
来源：http://aym.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mmg.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hcx.fehbvm.com

JS:   new Date();  Date.now()
来源：http://alo.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://gzl.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dme.316326.xyz

Go:   time.Now()
来源：http://day.316326.xyz

Ruby: Time.now
来源：http://pfy.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jdf.xinyue.icu

[J02] 格式化输出
来源：http://okz.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zlc.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qek.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lmk.sysykeji.top

TS:   d.toISOString()
来源：http://red.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gbf.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hgg.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://evj.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lbm.jinqigufen.top

[J03] 字符串解析为日期
来源：http://wcs.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tmr.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rcq.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://wtt.nanxinkj.top

TS:   new Date("2024-01-02")
来源：http://off.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://ize.shzxlz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sbu.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://rxq.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ata.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://tro.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gso.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://npp.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iml.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xfi.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://liw.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gca.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lyw.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kku.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://uab.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://zlm.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://bew.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://glp.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bza.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://bty.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pza.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://jrb.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://byk.jqgufenzy.top

[J06] 计算两时间之差
来源：http://qoj.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://szq.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://yfb.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nan.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://irp.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rqn.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://zwn.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://agu.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://bcv.zdqjudy.top

[J07] 比较两个日期
来源：http://wqe.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://jhd.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vfo.yanxiufei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://llk.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://yqb.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tvw.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ljm.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://mil.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://gle.aizwys.cn

[J08] 提取年月日与星期
来源：http://rvf.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qyj.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lap.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ftq.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://isi.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dbq.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://raw.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mha.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tav.yj20258888.top

[J09] 时区处理
来源：http://miy.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fgq.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vvf.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rff.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ihz.jinghuilouyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lid.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ntm.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rlq.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sow.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://ijt.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://knu.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bam.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zgn.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fae.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eiz.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wfh.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://boh.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jmj.yueranfly.top

================================================================================
来源：http://rad.hcnkem.com

K. JSON 与序列化
来源：http://rlz.guowangkeji.top

================================================================================
来源：http://dxq.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://aei.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dvr.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://anz.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://vet.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://wbu.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cqw.birdmap.top

Go:   json.Marshal(obj)
来源：http://hqa.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nzb.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://dgg.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://pgh.aizwys.cn

Py:   json.loads(s)
来源：http://gdi.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://njx.xylfe.cn

JS:   JSON.parse(s)
来源：http://mlv.sxryk.cn

TS:   JSON.parse(s)
来源：http://hwh.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rlw.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://lhf.daxiang520.top

Ruby: JSON.parse(s)
来源：http://iqo.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tvd.jianghu66.top

[K03] JSON 美化输出（带缩进）
来源：http://ulu.zdbjq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uzm.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cxt.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://vxb.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ldx.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://byt.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hrm.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://owf.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eby.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://qro.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://feq.hywenlv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xuu.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wbh.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://euk.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://brm.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eoa.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hov.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ykb.ivvv.top

[K05] 深拷贝对象
来源：http://giq.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://zph.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://jmp.52xcode.cn

JS:   structuredClone(obj)
来源：http://lks.zhengqikj.top

TS:   structuredClone(obj)
来源：http://pmn.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pzp.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://doj.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fih.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qdl.316326.xyz

[K06] 解析 URL 查询串
来源：http://lmv.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pka.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mao.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vkz.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ktt.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fwh.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://smv.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ymx.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zps.yongpay.top

[K07] 进制转换
来源：http://pgm.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qxh.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://har.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fem.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vji.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eeu.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bjg.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ioc.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jss.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://nau.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://uui.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://hwe.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://usa.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://nyu.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sob.tanke756.top

Go:   encoding/gob
来源：http://bqv.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://efo.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jto.zhiwuduotai.top

================================================================================
来源：http://kpj.kuanghao11.cn

L. 网络请求
来源：http://vmq.epnwcf.com

================================================================================
来源：http://jtz.dianchejie.cn

[L01] 发送 GET 请求
来源：http://pnr.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zvv.sxryk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sdv.dianchejie.cn

JS:   await fetch(url)
来源：http://uxg.jinqigfzy.top

TS:   await fetch(url)
来源：http://vej.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jsw.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://mwr.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://axo.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fjl.hnqzz.top

[L02] 发送 POST JSON
来源：http://ulw.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://gsq.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lrg.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wuf.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cyw.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://inr.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pxs.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cot.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zlk.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://ldq.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://snj.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gxr.bbcook.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dap.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emm.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xqj.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ios.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dus.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jek.chenzaomai.com

[L04] 设置超时
来源：http://hft.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://ijh.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cpo.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://coh.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lly.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oge.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nxk.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kcs.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zuq.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://jcx.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hll.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://koh.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xny.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ufd.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hwk.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oba.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ztk.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://alt.ehwqpu.com

[L06] 解析响应为 JSON
来源：http://ltx.quarkkingdee.top

Py:   resp.json()
来源：http://kzk.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://ygt.jianghu66.top

JS:   await resp.json()
来源：http://roh.xziqi.cn

TS:   await resp.json()
来源：http://mag.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://onk.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rqj.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://dpw.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://glh.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://xvk.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vzh.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cep.tanke756.top

JS:   resp.ok;  resp.status
来源：http://rca.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://xzo.yangfankeji.com

Java: resp.statusCode()
来源：http://wwm.havefunace.top

Go:   resp.StatusCode
来源：http://sdb.dashuyun.cn

Ruby: resp.code.to_i
来源：http://kwx.yj202588.top

C#:   (int)resp.StatusCode
来源：http://may.cucudq.cn

[L08] 并发请求多个地址
来源：http://pci.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hee.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://jnz.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nho.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tcg.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://olz.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wjo.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pgw.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rcy.ydzc1.top

================================================================================
来源：http://ixy.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://yzt.nanxuanxn.top


<!-- 参考信息 -->