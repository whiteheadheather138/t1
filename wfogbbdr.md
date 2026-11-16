代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://php.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://orp.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://cby.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://lgf.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://txr.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cha.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dws.epnwcf.com

[I05] 按正则拆分
来源：http://axa.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lwl.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blf.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://bpo.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://tli.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://hja.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ygx.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://bml.ybcxt.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ffi.c1oappe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ujy.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vdn.kuanghao11.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://epu.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://swt.zhongyouzk.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ghp.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dxw.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mfc.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rmy.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hyu.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://uzb.jyoumei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://psn.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zjh.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jcc.hcnkem.com

TS:   /error/gim
来源：http://njk.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hls.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yqd.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://dzd.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jko.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://rwu.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nqc.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ntb.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iac.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mlj.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://iih.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lqa.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bhw.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wde.jlsjyb.cn

================================================================================
来源：http://qfm.zhengqikj.top

J. 日期与时间
来源：http://ygb.hongshengwenyu.top

================================================================================
来源：http://iel.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://xem.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lcp.sufxvd.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zxp.sweek.top

JS:   new Date();  Date.now()
来源：http://imn.hammf.cn

TS:   new Date();  Date.now()
来源：http://ffq.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jjn.snrcjt.cn

Go:   time.Now()
来源：http://oxw.birdmap.top

Ruby: Time.now
来源：http://bbf.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://noz.vehdjk.com

[J02] 格式化输出
来源：http://rpe.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wil.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gbx.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qfl.feifeiyinyue.top

TS:   d.toISOString()
来源：http://tbw.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://huw.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tpx.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mrf.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vbx.bjfxy.top

[J03] 字符串解析为日期
来源：http://tur.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bgq.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bvm.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://wqt.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://hve.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://vaw.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jwm.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://dzg.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vyn.xylfe.cn

[J04] 时间戳与日期互转
来源：http://blm.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vki.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oyp.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ffi.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oat.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fmp.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wqq.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dax.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pvy.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://hjn.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://vhv.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://gbn.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hbc.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ttp.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://frr.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://doz.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://pij.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://qwi.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://tyt.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://wwa.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://lic.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lgs.ctjpmb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hpl.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xsf.hcnkem.com

Go:   end.Sub(start).Hours()
来源：http://trj.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://xun.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://axo.zhengqikj.top

[J07] 比较两个日期
来源：http://xsg.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://yop.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iei.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://uow.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://ext.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ljj.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jqc.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zxc.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://hyz.xuanzx.com

[J08] 提取年月日与星期
来源：http://vvs.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jwl.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://imx.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dqb.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://has.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bzo.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sua.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://adx.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eft.svipenyu.cn

[J09] 时区处理
来源：http://frv.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ros.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wmg.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vhm.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tqy.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gsg.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bpm.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nfj.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://brf.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://ulr.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cow.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oep.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xhq.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://srt.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ufo.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wit.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lgv.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wtt.uphjek.com

================================================================================
来源：http://cjo.zhiwuduotai.top

K. JSON 与序列化
来源：http://cct.hesvh.cn

================================================================================
来源：http://tzr.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://zya.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kmp.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wtd.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://boa.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://pfy.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uev.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://yph.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://kce.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gpw.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://rwp.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://xay.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vma.dashuyun.cn

JS:   JSON.parse(s)
来源：http://nck.meibo888.top

TS:   JSON.parse(s)
来源：http://keh.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dma.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://jef.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://trk.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fqz.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://tmn.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nfd.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://veo.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ten.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sug.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://maf.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://evj.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vaq.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vdu.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://mmv.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xwo.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fxz.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vep.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ehg.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yms.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xhg.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://vsk.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xek.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://jhb.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://axq.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://zjt.tianlin.xyz

JS:   structuredClone(obj)
来源：http://mlf.ctjpmb.com

TS:   structuredClone(obj)
来源：http://tav.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://akk.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://elr.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fhb.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hui.c1oappe.top

[K06] 解析 URL 查询串
来源：http://sub.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fju.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pwy.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qfb.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gjx.bjfxy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xid.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://eph.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://idu.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ovk.fzhhl.top

[K07] 进制转换
来源：http://ypi.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bqv.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yyi.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lot.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gsh.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kzv.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://abz.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zxn.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wbs.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://hpg.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://nqu.xuanzx.com

PHP:  serialize($obj);  unserialize($s);
来源：http://wou.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://suy.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://sad.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bnf.zhongyouzk.top

Go:   encoding/gob
来源：http://qje.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://pyb.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aut.tian-w.cn

================================================================================
来源：http://dzm.yongpay.top

L. 网络请求
来源：http://acw.vqdsnc.cn

================================================================================
来源：http://hfb.yj202588.top

[L01] 发送 GET 请求
来源：http://zzu.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kob.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rwx.pycfn.com

JS:   await fetch(url)
来源：http://dac.ivvv.top

TS:   await fetch(url)
来源：http://zxr.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hgo.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://ees.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://laj.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xcs.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://llk.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://tlv.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xfg.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://epj.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hxc.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zqt.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zsb.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qzt.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xby.gogol.net.cn

[L03] 设置自定义请求头
来源：http://rpn.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tip.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ulb.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://osn.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hij.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lij.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fcv.wangshuangyany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tmh.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lmt.snrcjt.cn

[L04] 设置超时
来源：http://irp.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://msf.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iby.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ewi.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://puc.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://boe.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gyg.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fwb.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pba.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://gfi.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sph.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zcy.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vfd.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xmm.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ipv.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ghd.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ewh.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rsq.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://zrq.fehbvm.com

Py:   resp.json()
来源：http://wrp.316326.xyz

PHP:  json_decode($body, true);
来源：http://pfn.jyoumei.cn

JS:   await resp.json()
来源：http://pfr.xziqi.cn

TS:   await resp.json()
来源：http://gkb.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ufo.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yfe.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://tej.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bxo.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://nuq.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lco.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wag.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://zmf.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://zjr.tanke756.top

Java: resp.statusCode()
来源：http://kzw.xylfe.cn

Go:   resp.StatusCode
来源：http://oqk.snrcjt.cn

Ruby: resp.code.to_i
来源：http://cqp.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://lba.sysykeji.top

[L08] 并发请求多个地址
来源：http://mqq.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cle.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://ooz.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vsy.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yqj.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ncc.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gnm.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kwc.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://irl.zycfv.cn

================================================================================
来源：http://evp.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://fuk.nanxinkj.top

================================================================================
来源：http://hpv.zdbjq.cn

[M01] 读取命令行参数
来源：http://cwb.yuanzhike.top

Py:   sys.argv[1:]
来源：http://fcn.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://eqe.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://ids.hammf.cn

TS:   process.argv.slice(2)
来源：http://dyy.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://xse.gzhubu.top

Go:   os.Args[1:]
来源：http://zas.feifeiyinyue.top

Ruby: ARGV
来源：http://pkw.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://bwr.zhixingplan.top

[M02] 读取环境变量
来源：http://fwb.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://ybv.yangfankeji.com


<!-- 参考信息 -->