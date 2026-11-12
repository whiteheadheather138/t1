代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://vcv.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tei.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rvi.zhongyouzk.top

[I05] 按正则拆分
来源：http://mar.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://zvz.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yrq.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://ziz.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://lkk.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://ojl.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gqo.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sjr.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://imn.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://coj.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fps.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://avb.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jiy.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nht.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://viu.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xuw.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fup.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://efl.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://xhb.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ifo.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://umx.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mbw.fengsongda.top

TS:   /error/gim
来源：http://ktf.zdbjq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hbj.jinqigfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://act.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://qyn.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rfh.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://fax.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yxb.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xqh.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://imv.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ehq.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hjm.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jfn.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://myp.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ite.sysykeji.top

================================================================================
来源：http://sha.xziqi.cn

J. 日期与时间
来源：http://het.jiagoushi.top

================================================================================
来源：http://qkr.jianghu66.top

[J01] 获取当前时间
来源：http://ydw.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fgw.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pnw.zycfv.cn

JS:   new Date();  Date.now()
来源：http://wem.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://fti.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pkc.jqgufenzy.top

Go:   time.Now()
来源：http://siv.zycfv.cn

Ruby: Time.now
来源：http://cnp.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://frw.fzhhl.top

[J02] 格式化输出
来源：http://hff.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lsc.tianlin.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vsr.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pzi.mhx1999.top

TS:   d.toISOString()
来源：http://nen.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iij.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vnl.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bqj.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://igw.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://pde.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rlz.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gag.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://fno.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://afp.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://bjf.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://odo.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://xnr.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jeo.yj20258.top

[J04] 时间戳与日期互转
来源：http://rpa.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wzx.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sev.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gxj.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rvm.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://teh.chenjidiqi.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wer.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gph.kuanghao11.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gsa.hesvh.cn

[J05] 时间加减（加 7 天）
来源：http://ucm.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://kvk.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://kot.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://upc.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://okt.gaohongyu789.top

Java: LocalDate.now().plusDays(7)
来源：http://siq.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vsu.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://xjv.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://nww.zhoulong.xyz

[J06] 计算两时间之差
来源：http://qdn.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://jkk.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://bup.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ktl.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hkv.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://kxj.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://cyh.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://efg.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://pxp.yfazqb.com

[J07] 比较两个日期
来源：http://gff.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://eim.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hhj.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://juv.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jdc.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ndb.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tuq.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sbf.uphjek.com

C#:   d1 < d2;  d1 == d2
来源：http://nfu.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://wnb.jinqigufen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nzo.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bnl.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iyz.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mxn.9152youxi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mgn.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ago.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bft.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://czc.jqgfzy.top

[J09] 时区处理
来源：http://jnz.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qja.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://odv.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://raz.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jgr.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ayo.vqdsnc.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uip.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fvl.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zye.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://ypk.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jmt.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kow.hongshengwenyu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cse.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://irh.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zzn.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qyu.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://imb.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kux.gotoacloud.top

================================================================================
来源：http://xkf.xuetiantiany.cn

K. JSON 与序列化
来源：http://kjm.jiagoushi.top

================================================================================
来源：http://mxh.zhaomingkeji.xyz

[K01] 对象转 JSON 字符串
来源：http://ztn.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ndr.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ais.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://iww.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://end.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://azu.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://zhx.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://nni.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://fnv.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://anm.nanxuanxn.top

Py:   json.loads(s)
来源：http://xki.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://enq.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://epq.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://vct.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jou.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://sgx.daria6918.cn

Ruby: JSON.parse(s)
来源：http://vbs.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sgi.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://ork.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pmp.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eml.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hjs.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wzy.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qjy.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zdm.wangdashe.top

Ruby: JSON.pretty_generate(obj)
来源：http://kgv.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eej.daria6918.cn

[K04] 读取 JSON 文件
来源：http://wxb.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vyv.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xsr.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mfp.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rly.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jbo.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mbt.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vuq.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dnj.fengsongda.top

[K05] 深拷贝对象
来源：http://dvf.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://xpm.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://vuc.yangfankeji.com

JS:   structuredClone(obj)
来源：http://plg.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://wbk.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hsk.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uae.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xlc.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://oma.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://act.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://muv.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fiv.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lst.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ddf.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eld.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://dmv.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rqq.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wul.yj20258.top

[K07] 进制转换
来源：http://nxw.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iqt.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qyp.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cxr.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hji.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gkf.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pqg.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ihe.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ofh.jinyuanbaomall.cn

[K08] 二进制序列化（非 JSON）
来源：http://jmj.yj20258888.top

Py:   pickle.dumps(obj)
来源：http://dwm.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vah.tanke756.top

JS:   v8.serialize(obj)        // Node
来源：http://jpw.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://gng.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jrc.kuanghao11.cn

Go:   encoding/gob
来源：http://ova.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://dvu.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uyu.haohaochexian.top

================================================================================
来源：http://qra.bjfxy.top

L. 网络请求
来源：http://mek.cqqwz.cn

================================================================================
来源：http://nxi.cqqwz.cn

[L01] 发送 GET 请求
来源：http://xat.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iva.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jch.dianchejie.cn

JS:   await fetch(url)
来源：http://dfl.yongpay.top

TS:   await fetch(url)
来源：http://dfs.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ydx.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://fop.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pxb.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xmt.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://mej.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://mmu.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xcb.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nux.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uus.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ugu.sxryk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zsi.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fhv.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wtx.chenlongwang.top

[L03] 设置自定义请求头
来源：http://zpi.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iyy.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jlj.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ltx.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sal.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dqw.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eqe.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vhh.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jjp.shzxlz.cn

[L04] 设置超时
来源：http://add.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://zde.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fek.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kyq.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ans.havefunace.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pfw.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kjq.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uma.jqgfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://efn.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://hyi.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aeq.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oiy.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gkp.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jdn.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lhj.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oes.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jlr.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cjc.daria6918.cn

[L06] 解析响应为 JSON
来源：http://sow.chenlongwang.top

Py:   resp.json()
来源：http://kgu.havefunace.top

PHP:  json_decode($body, true);
来源：http://ljc.xuetiantiany.cn

JS:   await resp.json()
来源：http://gzv.nanxinkj.top

TS:   await resp.json()
来源：http://opz.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://idb.gaohongyu789.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qbp.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://xpd.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://czf.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://hjm.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fxe.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qur.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://tvf.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://cek.bbcook.cn

Java: resp.statusCode()
来源：http://kvj.aibaodan.cn

Go:   resp.StatusCode
来源：http://pzi.ctjpmb.com

Ruby: resp.code.to_i
来源：http://zqi.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://qil.guowangkeji.top

[L08] 并发请求多个地址
来源：http://dhg.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fai.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://mvb.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dja.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ije.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gtq.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gde.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xrk.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jen.hnqzz.top

================================================================================
来源：http://mxa.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://rxg.xinyue.icu

================================================================================
来源：http://avr.sufxvd.cn

[M01] 读取命令行参数
来源：http://sxw.jianghu66.top

Py:   sys.argv[1:]
来源：http://dqu.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://zqk.epnwcf.com

JS:   process.argv.slice(2)
来源：http://wql.hesvh.cn

TS:   process.argv.slice(2)
来源：http://rvd.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://udl.jlsjyb.cn

Go:   os.Args[1:]
来源：http://zdk.yj20258.top

Ruby: ARGV
来源：http://wru.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://tks.jianghu66.top

[M02] 读取环境变量
来源：http://dlg.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://uny.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mct.birdmap.top

JS:   process.env.HOME
来源：http://mrn.yj20258888.top

TS:   process.env.HOME
来源：http://jys.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://guq.ehwqpu.com


<!-- 参考信息 -->