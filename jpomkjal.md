代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xwp.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hcd.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mbl.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wlb.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qfv.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dni.zhongyouzk.top

[I04] 正则替换
来源：http://msc.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lus.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ykd.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://abc.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jpe.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://ify.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lkv.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pkz.jiagoushi.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dhn.jinqigfzy.top

[I05] 按正则拆分
来源：http://wng.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tdd.jinghuilouyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ytu.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://tca.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://fkr.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://nua.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rqi.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://yfu.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iwl.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wlp.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qpe.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tff.sysykeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://abt.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eqy.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uwb.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ypw.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ymz.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bpl.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://uxn.0kj1m.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bfj.svipenyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://egg.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iiz.kuanghao11.cn

TS:   /error/gim
来源：http://kee.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tfo.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xjk.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://nts.xylfe.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://goh.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://nfe.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ojm.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kkq.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ind.bbcook.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xnf.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://czl.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qkj.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://apv.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gsq.sjlbkw.cn

================================================================================
来源：http://mya.andypj.xyz

J. 日期与时间
来源：http://jul.yongpay.top

================================================================================
来源：http://dzb.9152youxi.cn

[J01] 获取当前时间
来源：http://tsk.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jje.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://drr.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://hrl.316326.xyz

TS:   new Date();  Date.now()
来源：http://qhc.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kuo.meibo888.top

Go:   time.Now()
来源：http://gxl.vqdsnc.cn

Ruby: Time.now
来源：http://wvh.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ifh.hysaishi.cn

[J02] 格式化输出
来源：http://jgw.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wii.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://whr.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fyp.jinqigfzy.top

TS:   d.toISOString()
来源：http://bar.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nok.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cre.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tbv.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nsv.guowangkeji.top

[J03] 字符串解析为日期
来源：http://ltz.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gvg.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iis.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://tzz.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://xny.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://sgh.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nyw.9152youxi.cn

Ruby: Date.parse("2024-01-02")
来源：http://mfs.cdnleiting.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bse.xuanzx.com

[J04] 时间戳与日期互转
来源：http://nzm.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kvl.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hcd.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ldd.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://xic.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://anf.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://asx.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://svj.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lpm.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://xmk.meibo888.top

Py:   now + timedelta(days=7)
来源：http://mvm.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://era.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oma.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yve.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://vyp.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zyu.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://wzt.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://esw.0kj1m.cn

[J06] 计算两时间之差
来源：http://kyy.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://utj.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://fxw.zhaomingkeji.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xod.ydzc1.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jhm.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://jug.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://xwd.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://ivu.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://ofs.jinqigfzy.top

[J07] 比较两个日期
来源：http://kfg.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://bww.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uye.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://pfh.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rnq.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jdj.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://csm.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pyo.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://inm.chenzaomai.com

[J08] 提取年月日与星期
来源：http://tnl.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fdk.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vxn.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nmv.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://djo.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jih.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://its.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pqo.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ynw.ppjwa.cn

[J09] 时区处理
来源：http://qxs.zhixingplan.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wgh.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jjr.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cel.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xxa.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gxd.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ojp.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qdp.sufxvd.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zqa.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://kmn.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zeg.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xyx.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://puh.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ssd.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qyp.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ujo.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kkf.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qfx.chenzaomai.com

================================================================================
来源：http://rqu.9152youxi.cn

K. JSON 与序列化
来源：http://bgx.shuidangran.top

================================================================================
来源：http://ccr.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://roz.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ngl.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nox.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://lgd.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://qgr.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://loo.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://hee.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://yfz.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cez.sxryk.cn

[K02] JSON 字符串转对象
来源：http://ipo.tarul.cn

Py:   json.loads(s)
来源：http://jle.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mxm.haohaochexian.top

JS:   JSON.parse(s)
来源：http://enk.xuanzx.com

TS:   JSON.parse(s)
来源：http://crt.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://egz.316326.xyz

Go:   json.Unmarshal(data, &v)
来源：http://vcf.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://tcq.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://phe.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://iax.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://umb.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hrp.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://etz.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://aaf.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://srz.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gxw.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://rat.guowangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pvy.gzhubu.top

[K04] 读取 JSON 文件
来源：http://zzq.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ett.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cxk.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://egm.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vyr.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tup.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nob.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mue.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jwa.zhengqikj.top

[K05] 深拷贝对象
来源：http://oxt.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://tfm.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://tod.yfazqb.com

JS:   structuredClone(obj)
来源：http://xso.tian-w.cn

TS:   structuredClone(obj)
来源：http://dsn.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ajf.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://csg.hnqzz.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pdx.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dav.daria6918.cn

[K06] 解析 URL 查询串
来源：http://yky.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hii.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://epb.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rpr.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iod.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://woe.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xcc.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dbi.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xzg.jinyuanbaomall.cn

[K07] 进制转换
来源：http://xkz.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eld.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hla.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dlo.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pos.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iaz.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://toi.dianchejie.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://roc.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ffh.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://xro.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://wnd.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://psd.havefunace.top

JS:   v8.serialize(obj)        // Node
来源：http://inv.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://cpk.hcnkem.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pjp.aizwys.cn

Go:   encoding/gob
来源：http://phh.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://lho.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qcy.cheryme.top

================================================================================
来源：http://wsd.xziqi.cn

L. 网络请求
来源：http://pcp.pycfn.com

================================================================================
来源：http://hsp.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://asf.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gar.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sat.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://rio.316326.xyz

TS:   await fetch(url)
来源：http://hgd.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qfx.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://rxw.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://muw.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gta.xuanzx.com

[L02] 发送 POST JSON
来源：http://gdi.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://eay.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jpk.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iay.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cch.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lql.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xec.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jac.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ovv.yfazqb.com

[L03] 设置自定义请求头
来源：http://vlf.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xvl.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uys.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ucc.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dbm.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://efc.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jgd.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://okv.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zdo.uphjek.com

[L04] 设置超时
来源：http://psn.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://fyy.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zig.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wyw.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://thw.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fet.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xxw.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kvx.jinqigufen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rez.jianghu66.top

[L05] 上传文件（multipart）
来源：http://eut.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ppb.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vai.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://prl.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yok.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rsn.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxk.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://olm.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rms.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://yzt.mhx1999.top

Py:   resp.json()
来源：http://vti.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://iio.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://tlo.fengsongda.top

TS:   await resp.json()
来源：http://rxy.0kj1m.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hpm.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://joq.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://zrv.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fdo.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://pdo.xinyue.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://neg.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tyg.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://cat.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://okm.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://vmw.0kj1m.cn

Go:   resp.StatusCode
来源：http://ahs.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://tmw.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://gic.yongpay.top

[L08] 并发请求多个地址
来源：http://kcn.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fhm.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://ucm.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yux.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qkc.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pji.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ctp.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xfb.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mdr.xylfe.cn

================================================================================
来源：http://sjk.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://dif.shzxlz.cn

================================================================================
来源：http://tdf.tian-w.cn

[M01] 读取命令行参数
来源：http://zxo.tian-w.cn

Py:   sys.argv[1:]
来源：http://ljd.fktsv.cn

PHP:  $argv;  $argc;
来源：http://pdt.hywenlv.cn


<!-- 参考信息 -->