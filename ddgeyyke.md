代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zzq.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cvc.hesvh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ijr.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kxg.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://icv.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rhr.havefunace.top

[I04] 正则替换
来源：http://vzv.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ado.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ifk.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://rfr.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://aum.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qih.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qhf.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://nmq.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nzp.yonumen.top

[I05] 按正则拆分
来源：http://lfc.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lgt.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uvz.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://pon.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://yjq.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://npy.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bli.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://xjd.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://izg.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kts.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wyb.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yva.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sfw.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ozm.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wmz.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://npj.cheryme.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jrh.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://apn.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://jcd.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://quj.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gdj.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iql.ydjk.org.cn

TS:   /error/gim
来源：http://ubl.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://igo.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://npw.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://tby.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cyp.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://lpy.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://djh.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pdv.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jhc.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://czw.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bdy.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uic.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jyl.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aqb.cqqwz.cn

================================================================================
来源：http://qoz.yongpay.top

J. 日期与时间
来源：http://cps.jinyuanbaomall.cn

================================================================================
来源：http://isr.mhx1999.top

[J01] 获取当前时间
来源：http://rvv.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ywp.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hgu.fktsv.cn

JS:   new Date();  Date.now()
来源：http://jdi.tarul.cn

TS:   new Date();  Date.now()
来源：http://nqa.gotoacloud.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hdp.nanxuanxn.top

Go:   time.Now()
来源：http://qhj.yfazqb.com

Ruby: Time.now
来源：http://ukp.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lyc.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://ltz.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dbs.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lza.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iit.jinqigufen.top

TS:   d.toISOString()
来源：http://ded.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://atk.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cbu.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kab.ywan-chungtsiang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nue.wangdashe.top

[J03] 字符串解析为日期
来源：http://cty.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://htv.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wfz.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://iar.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://tqt.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://ymg.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mhx.pycfn.com

Ruby: Date.parse("2024-01-02")
来源：http://lqu.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ppc.xziqi.cn

[J04] 时间戳与日期互转
来源：http://kel.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uhu.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ydk.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vhr.epnwcf.com

TS:   Math.floor(Date.now() / 1000)
来源：http://sns.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nhx.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mcb.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mnh.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fto.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://nhs.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://epv.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ecx.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tlh.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mjr.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://xoj.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://shb.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://znj.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://oew.yfazqb.com

[J06] 计算两时间之差
来源：http://uha.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://kbv.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://dab.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kwd.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pmu.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gma.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://npz.tian-w.cn

Ruby: end - start                 # 返回秒数
来源：http://nrq.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://eky.vqdsnc.cn

[J07] 比较两个日期
来源：http://qot.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://ldy.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://inp.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://ggv.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://gjx.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uze.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nhx.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://aas.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://qgi.shzxlz.cn

[J08] 提取年月日与星期
来源：http://zfa.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jee.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://knb.jinyuanbaomall.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rce.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yml.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rni.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sjz.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mat.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wgb.jyoumei.cn

[J09] 时区处理
来源：http://wpx.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yrw.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nqz.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pkr.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ebp.wangdashe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aca.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bro.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xch.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kqd.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://axd.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://plr.cucudq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wci.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zna.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eqe.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ovw.jqgfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zkl.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tcg.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ndd.dashuyun.cn

================================================================================
来源：http://tud.snrcjt.cn

K. JSON 与序列化
来源：http://vbq.ywan-chungtsiang.top

================================================================================
来源：http://fpg.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://quo.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mgh.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ryw.yonumen.top

JS:   JSON.stringify(obj)
来源：http://blh.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://cqy.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aet.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://cek.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://wmc.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dzx.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://nck.zycfv.cn

Py:   json.loads(s)
来源：http://bzg.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://orb.wangdashe.top

JS:   JSON.parse(s)
来源：http://dtw.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://ciy.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://feq.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://kls.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://szc.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tof.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://xtr.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pvs.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bjp.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://laa.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ovi.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rkf.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kfi.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://jjp.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://osw.ivvv.top

[K04] 读取 JSON 文件
来源：http://eff.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mic.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wgy.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yqx.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qer.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lbq.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pzv.yuanzhike.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://veg.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kev.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://jyp.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://sqv.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://vjj.kuanghao11.cn

JS:   structuredClone(obj)
来源：http://xnq.daria6918.cn

TS:   structuredClone(obj)
来源：http://erd.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qiz.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jkn.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ntj.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://sip.cucudq.cn

[K06] 解析 URL 查询串
来源：http://bfb.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hsi.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://irb.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lmb.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zcw.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mfe.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bei.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kde.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bvd.gzhubu.top

[K07] 进制转换
来源：http://uwr.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bpr.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zqu.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bby.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uof.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yab.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mco.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qtp.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mxs.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://ijc.tianlin.xyz

Py:   pickle.dumps(obj)
来源：http://jpc.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wlo.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://ldu.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://yli.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zno.yonumen.top

Go:   encoding/gob
来源：http://jni.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://umv.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pyi.zhaomingkeji.xyz

================================================================================
来源：http://sjm.tarul.cn

L. 网络请求
来源：http://wiy.fzhhl.top

================================================================================
来源：http://ote.fzhhl.top

[L01] 发送 GET 请求
来源：http://eys.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xsl.zdbjq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vco.pengpengdd.cyou

JS:   await fetch(url)
来源：http://bdn.yanxiufei.cn

TS:   await fetch(url)
来源：http://gdc.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uqr.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://gan.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://epu.zycfv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://efa.mhx1999.top

[L02] 发送 POST JSON
来源：http://grh.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dcj.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xra.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ips.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mvj.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vkk.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uyt.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fcu.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tzi.yuxming.cn

[L03] 设置自定义请求头
来源：http://xqg.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ain.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lvh.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kiy.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nep.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gpa.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kan.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vnw.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oej.wangshuangyany.cn

[L04] 设置超时
来源：http://ojm.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://sci.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tmb.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rqn.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pot.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rpo.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lck.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ako.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://thc.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://xyt.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xtf.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rtr.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wim.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lki.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://azu.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rae.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bvb.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pld.316326.xyz

[L06] 解析响应为 JSON
来源：http://pke.xinyue.icu

Py:   resp.json()
来源：http://fff.hysaishi.cn

PHP:  json_decode($body, true);
来源：http://ivu.hfpthk.cn

JS:   await resp.json()
来源：http://vmf.xuetiantiany.cn

TS:   await resp.json()
来源：http://jew.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oka.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://okf.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://dya.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lbp.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://vgd.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yut.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ovq.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://yrj.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://koq.jiagoushi.top

Java: resp.statusCode()
来源：http://hjj.chenzaomai.com

Go:   resp.StatusCode
来源：http://hgq.sweek.top

Ruby: resp.code.to_i
来源：http://yzx.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://pja.yj20258.top

[L08] 并发请求多个地址
来源：http://dxx.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bzc.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://zaq.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xlo.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bxb.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mcq.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yyv.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://juc.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://als.xingfuxueyuan.xyz

================================================================================
来源：http://vjc.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://tgs.nanxinkj.top

================================================================================
来源：http://owl.chenzaomai.com

[M01] 读取命令行参数
来源：http://qla.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://eqh.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://xgu.jinqigfzy.top


<!-- 参考信息 -->