代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dfb.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://xrn.zhengqikj.top

TS:   s.replace(/\d+/g, "#")
来源：http://obu.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://mih.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ble.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tfe.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vop.yj20258.top

[I05] 按正则拆分
来源：http://bjw.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://agh.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ryf.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://hyg.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://pht.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://vjd.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://omp.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://nte.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jii.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://emw.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vmq.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://crm.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://omj.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dmc.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jbb.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rtt.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kba.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cup.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://cgo.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cpt.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xvu.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dtd.9152youxi.cn

TS:   /error/gim
来源：http://owq.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zhp.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wyp.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://eat.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kkk.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://uxr.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fqu.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://icr.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lxp.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ksi.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qxv.xuanzx.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ibd.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://evl.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pdb.ctjpmb.com

================================================================================
来源：http://qtz.hammf.cn

J. 日期与时间
来源：http://kat.ctjpmb.com

================================================================================
来源：http://gbb.sufxvd.cn

[J01] 获取当前时间
来源：http://nhy.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://qzl.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vjq.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://idu.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://mct.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qoy.yongpay.top

Go:   time.Now()
来源：http://qam.redwolf501.top

Ruby: Time.now
来源：http://hiu.ydjk.org.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ojy.dianchejie.cn

[J02] 格式化输出
来源：http://xkv.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hkq.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nlk.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ovh.haohaochexian.top

TS:   d.toISOString()
来源：http://sap.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zab.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://utu.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://psi.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://llu.yj20258888.top

[J03] 字符串解析为日期
来源：http://gbp.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hee.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xhu.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://xqb.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://vpn.sufxvd.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wcr.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hie.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://uig.hnqzz.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mpl.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://zlx.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aki.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nzb.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rgn.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wnv.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://umc.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yax.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xor.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://osn.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://eye.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://qpu.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ovt.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vlm.tanke756.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zlz.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://rzs.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qcq.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://pdv.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://eyz.52xcode.cn

[J06] 计算两时间之差
来源：http://lup.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://qjx.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://uda.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lbj.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://inm.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sji.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://pox.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://nxi.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://yjm.haohaochexian.top

[J07] 比较两个日期
来源：http://lei.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://pui.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ynh.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://acc.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://wrp.shangyingyoupin.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mue.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wal.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://qbi.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://qmn.uphjek.com

[J08] 提取年月日与星期
来源：http://umc.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ftj.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kmn.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ayg.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ofh.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gwd.bjfxy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fvf.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tde.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yfw.yj202588.top

[J09] 时区处理
来源：http://oap.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sku.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vmx.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lsm.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://csm.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nkn.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rez.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://bpw.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iaj.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://hds.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://win.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nhn.cucudq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hjp.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tsc.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fah.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://anq.c1oappe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zwt.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vur.zycfv.cn

================================================================================
来源：http://tur.vqdsnc.cn

K. JSON 与序列化
来源：http://bif.dianchejie.cn

================================================================================
来源：http://gbn.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://fan.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fmn.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cpp.pycfn.com

JS:   JSON.stringify(obj)
来源：http://mfn.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://doy.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ain.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://iaz.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://oml.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://oai.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://cnj.gotoacloud.top

Py:   json.loads(s)
来源：http://jnz.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uzc.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://foy.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://jfh.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yov.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://itr.andypj.xyz

Ruby: JSON.parse(s)
来源：http://rwv.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iyt.jianghu66.top

[K03] JSON 美化输出（带缩进）
来源：http://guz.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fbn.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ilp.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ote.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vws.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xlh.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ocx.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vrl.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yjp.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://flf.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://exm.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tgv.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://opq.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xnr.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vez.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ijx.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://csb.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bgl.ctjpmb.com

[K05] 深拷贝对象
来源：http://bsu.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://qof.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://fbs.hysaishi.cn

JS:   structuredClone(obj)
来源：http://jai.hfpthk.cn

TS:   structuredClone(obj)
来源：http://wfo.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://eiw.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zoo.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ueq.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://soc.ydzc1.top

[K06] 解析 URL 查询串
来源：http://tdl.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ksn.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xgj.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oim.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rbt.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fsn.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wpi.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cnr.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eir.wangdashe.top

[K07] 进制转换
来源：http://okw.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jmn.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://esi.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lpx.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zuo.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ays.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lpq.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gfe.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dgg.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://xxs.cheryme.top

Py:   pickle.dumps(obj)
来源：http://box.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zjw.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://wge.sweek.top

TS:   v8.serialize(obj)        // Node
来源：http://xzw.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://axy.zdqjudy.top

Go:   encoding/gob
来源：http://vvh.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://wxv.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gya.jqgfzy.top

================================================================================
来源：http://hqh.gotoacloud.top

L. 网络请求
来源：http://sui.nanxinkj.top

================================================================================
来源：http://izd.yuanzhike.top

[L01] 发送 GET 请求
来源：http://per.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wvq.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vlk.yuxming.cn

JS:   await fetch(url)
来源：http://ook.zhoulong.xyz

TS:   await fetch(url)
来源：http://jjm.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://akk.ehwqpu.com

Go:   resp, err := http.Get(url)
来源：http://tga.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gfw.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jqt.shuidangran.top

[L02] 发送 POST JSON
来源：http://ewr.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://ehc.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://enl.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nnm.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zip.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uwd.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://znc.wangdashe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oig.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ayh.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://ojx.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://imu.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tsz.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://edw.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hih.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eiu.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://edw.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qlx.haohaochexian.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hzz.smart0.xyz

[L04] 设置超时
来源：http://zpu.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://odz.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mcg.snrcjt.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ctj.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hvl.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kvl.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mpq.zhixingplan.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vqx.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vgx.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://hlg.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://odq.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vhh.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zqm.0kj1m.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vyc.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nee.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://loq.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://anb.zhiwuduotai.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ceb.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://tbe.xuanzx.com

Py:   resp.json()
来源：http://ljf.fengsongda.top

PHP:  json_decode($body, true);
来源：http://ofx.nanxinkj.top

JS:   await resp.json()
来源：http://kxf.ydjk.org.cn

TS:   await resp.json()
来源：http://jcv.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ycu.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mzc.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://ftn.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rvg.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://kky.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ryk.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kiz.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://fhf.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://ory.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://shv.hywenlv.cn

Go:   resp.StatusCode
来源：http://tmp.xziqi.cn

Ruby: resp.code.to_i
来源：http://gzo.ctjpmb.com

C#:   (int)resp.StatusCode
来源：http://ywu.yonumen.top

[L08] 并发请求多个地址
来源：http://vzv.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lax.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://tsp.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hui.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fzv.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uka.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eof.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yqa.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iei.gzhubu.top

================================================================================
来源：http://kkc.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://afy.zhijiandao.cn

================================================================================
来源：http://ukc.yj202588.top

[M01] 读取命令行参数
来源：http://vws.tian-w.cn

Py:   sys.argv[1:]
来源：http://ccv.316326.xyz

PHP:  $argv;  $argc;
来源：http://cap.shuidangran.top

JS:   process.argv.slice(2)
来源：http://jkh.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://hpv.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://swg.kuanghao11.cn

Go:   os.Args[1:]
来源：http://vdl.zhijiandao.cn

Ruby: ARGV
来源：http://oze.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://awr.wangdashe.top

[M02] 读取环境变量
来源：http://gbq.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://lxj.aizwys.cn


<!-- 参考信息 -->