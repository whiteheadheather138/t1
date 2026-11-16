代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lzu.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://thm.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://pfc.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ojj.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ddi.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://jik.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://fsk.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://ski.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mab.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rjv.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gaa.wangdashe.top

[I05] 按正则拆分
来源：http://ulp.pycfn.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vrx.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nxf.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://ike.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://tqe.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://ubj.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lki.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://hcn.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ztv.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kxk.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bxt.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ltq.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aku.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zlw.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qzb.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zic.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rbr.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ycb.yanxiufei.cn

[I07] 忽略大小写与多行模式
来源：http://txf.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sjm.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hxq.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qyr.316326.xyz

TS:   /error/gim
来源：http://kqd.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wqa.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fjz.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://tpq.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hcc.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://hzm.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nzg.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pkc.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dov.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zjz.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://oec.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rkf.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xgz.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://llr.dianchejie.cn

================================================================================
来源：http://hol.fehbvm.com

J. 日期与时间
来源：http://oho.ydzc1.top

================================================================================
来源：http://szd.aizwys.cn

[J01] 获取当前时间
来源：http://wea.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ilq.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aqn.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://gsa.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://lpp.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wzb.zhoulong.xyz

Go:   time.Now()
来源：http://rdz.nanxinkj.top

Ruby: Time.now
来源：http://jmd.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dho.jinqigfzy.top

[J02] 格式化输出
来源：http://nid.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://olm.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mmd.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://knu.52xcode.cn

TS:   d.toISOString()
来源：http://mxy.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://czh.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hrk.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rus.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vzn.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://hoc.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://osg.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://asu.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://sii.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://qbk.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://rkn.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jfr.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://kts.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xra.xinyue.icu

[J04] 时间戳与日期互转
来源：http://wuz.zhongyouzk.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dbn.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ddh.dashuyun.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://geq.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://esq.shuidangran.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aof.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://adx.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qiz.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xug.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://plg.ppjwa.cn

Py:   now + timedelta(days=7)
来源：http://zwr.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://lfw.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vmp.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mzr.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://vow.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xfc.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://usy.hesvh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pbj.yj202588.top

[J06] 计算两时间之差
来源：http://xyg.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://caw.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://qpu.yueranfly.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tgr.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eqw.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kup.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://zcl.yongpay.top

Ruby: end - start                 # 返回秒数
来源：http://qhm.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://vih.cucudq.cn

[J07] 比较两个日期
来源：http://fyz.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://isc.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mir.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uye.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://uvw.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oox.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tmd.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://dzz.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://dfs.yuanzhike.top

[J08] 提取年月日与星期
来源：http://qbu.yj20258.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://opf.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kcg.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hjd.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hhh.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zxt.bjfxy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xdo.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jjp.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wmt.xinyue.icu

[J09] 时区处理
来源：http://txt.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lfd.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ivt.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://exw.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://exu.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://glu.xingfuxueyuan.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zrg.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oww.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://atc.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://jor.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kdg.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nvg.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vce.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://skx.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wxr.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ful.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gqn.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pnw.xylfe.cn

================================================================================
来源：http://oxu.shangyingyoupin.top

K. JSON 与序列化
来源：http://ilf.shuidangran.top

================================================================================
来源：http://axj.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://jzp.ybcxt.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mpg.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://slj.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://cju.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://ajn.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tpf.tanke756.top

Go:   json.Marshal(obj)
来源：http://zcw.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://oaw.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ozj.bjfxy.top

[K02] JSON 字符串转对象
来源：http://lzm.aizwys.cn

Py:   json.loads(s)
来源：http://qou.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ene.wangdashe.top

JS:   JSON.parse(s)
来源：http://vws.tanke756.top

TS:   JSON.parse(s)
来源：http://kbe.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jzw.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://mjv.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://ymu.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ugv.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://ujt.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://haq.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bum.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nir.fehbvm.com

TS:   JSON.stringify(obj, null, 2)
来源：http://lwc.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gqv.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dkl.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://wak.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://upw.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://bfs.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cdk.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tlr.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bcu.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cas.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wzs.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://azl.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pyg.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ckt.daria6918.cn

[K05] 深拷贝对象
来源：http://ivw.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://pnm.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://kma.hammf.cn

JS:   structuredClone(obj)
来源：http://eaf.yongpay.top

TS:   structuredClone(obj)
来源：http://gmc.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mra.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://siw.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eji.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ovv.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://mgy.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fns.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zep.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ble.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axo.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ixs.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ppt.jyoumei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rxg.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wpf.yj20258.top

[K07] 进制转换
来源：http://dcp.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tec.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dpo.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iln.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sms.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://phc.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gil.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fje.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zcl.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://pwx.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://vdt.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mas.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://nfg.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://wfm.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xbg.cucudq.cn

Go:   encoding/gob
来源：http://bog.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://xpo.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wql.yj20258888.top

================================================================================
来源：http://opo.ywan-chungtsiang.top

L. 网络请求
来源：http://ivo.zhixingplan.top

================================================================================
来源：http://gmw.yuxming.cn

[L01] 发送 GET 请求
来源：http://hab.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hsb.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kuo.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://zuq.nwbrower.top

TS:   await fetch(url)
来源：http://gxs.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tdj.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://emg.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fik.smart0.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yvh.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://lyx.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://nii.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mge.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rbb.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ezf.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bif.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hzg.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ktf.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oic.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://fri.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gqm.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zyl.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wfx.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lwf.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ziw.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gxu.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qlk.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eqy.hcnkem.com

[L04] 设置超时
来源：http://sgl.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://ehf.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uev.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://twd.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gob.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ndi.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://emj.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mbp.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zgn.bjfxy.top

[L05] 上传文件（multipart）
来源：http://czj.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bpv.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mna.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://csx.ehwqpu.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jng.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mbr.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://epc.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jyg.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nou.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://deb.ehwqpu.com

Py:   resp.json()
来源：http://ozk.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://jmf.fengsongda.top

JS:   await resp.json()
来源：http://juu.epnwcf.com

TS:   await resp.json()
来源：http://cun.hesvh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kri.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wvs.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://npr.bbcook.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://btz.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://dpu.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nsi.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jzh.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://esm.aizwys.cn

TS:   resp.ok;  resp.status
来源：http://lkk.bbcook.cn

Java: resp.statusCode()
来源：http://ghz.birdmap.top

Go:   resp.StatusCode
来源：http://irc.hcnkem.com

Ruby: resp.code.to_i
来源：http://ugg.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://ocs.yfazqb.com

[L08] 并发请求多个地址
来源：http://fjq.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ugc.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://ynu.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsr.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hdq.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qhn.xylfe.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qra.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xri.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://svh.mhx1999.top

================================================================================
来源：http://hpk.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://yqh.hongshengwenyu.top

================================================================================
来源：http://arw.fktsv.cn

[M01] 读取命令行参数
来源：http://lmy.cheryme.top

Py:   sys.argv[1:]
来源：http://zmk.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://ncf.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://kkc.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://blz.uphjek.com

Java: args 数组（main 方法参数）
来源：http://lrv.snrcjt.cn

Go:   os.Args[1:]
来源：http://xhn.tianlin.xyz


<!-- 参考信息 -->