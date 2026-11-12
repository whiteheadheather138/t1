代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://kvc.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ctv.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://jlo.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tbn.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kyx.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pbh.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rla.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nap.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbb.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wol.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://frn.bjfxy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xfu.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tfq.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://aon.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qnc.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hdf.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dsg.jiagoushi.top

TS:   /error/gim
来源：http://ouf.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wze.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zto.yj202588.top

Ruby: s.scan(/error/i)
来源：http://hvo.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mev.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://ueh.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://deq.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kgs.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxk.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cin.haohaochexian.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rmg.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bry.sufxvd.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pcx.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nay.fzhhl.top

================================================================================
来源：http://uvr.ywan-chungtsiang.top

J. 日期与时间
来源：http://ass.chenlongwang.top

================================================================================
来源：http://ufs.sysykeji.top

[J01] 获取当前时间
来源：http://xya.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ruq.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bsa.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://aui.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://imw.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kuf.gotoacloud.top

Go:   time.Now()
来源：http://vec.yonumen.top

Ruby: Time.now
来源：http://cyb.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bor.daxiang520.top

[J02] 格式化输出
来源：http://ecb.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lmp.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bby.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wsn.birdmap.top

TS:   d.toISOString()
来源：http://xiy.jyoumei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://csl.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://whz.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zdx.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blk.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://tln.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aqw.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ggm.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://ygh.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://vls.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uug.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vte.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://icu.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zyj.52xcode.cn

[J04] 时间戳与日期互转
来源：http://xzd.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zus.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dre.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xyj.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://tkz.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pkt.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fiw.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pmd.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://myt.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://xuv.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://vvl.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pcc.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cxz.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rta.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://ehh.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gyg.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://oqv.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vwf.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://ncj.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://epu.tarul.cn

PHP:  $end->diff($start)->days;
来源：http://lhk.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bpn.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ele.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://vew.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://jtb.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://hcd.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://fkz.tian-w.cn

[J07] 比较两个日期
来源：http://guh.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://tzs.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dwn.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://uke.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://htl.jinghuilouyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aef.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hvu.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://avk.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://isc.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://bwx.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mah.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oxe.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xzk.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://drs.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://svl.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kli.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zyj.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uer.ctjpmb.com

[J09] 时区处理
来源：http://akp.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qfb.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oux.zdbjq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qpw.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oni.guowangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ljz.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vvx.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xju.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jky.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://zuu.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oyw.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://thx.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vri.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://umv.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xus.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tmz.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://slp.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ago.meibo888.top

================================================================================
来源：http://ipx.bbcook.cn

K. JSON 与序列化
来源：http://wgm.ywan-chungtsiang.top

================================================================================
来源：http://mnj.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://slm.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gvd.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zoc.yongpay.top

JS:   JSON.stringify(obj)
来源：http://bao.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://lzo.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gyh.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://euo.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://fnb.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://coj.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://rpe.cucudq.cn

Py:   json.loads(s)
来源：http://bbp.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://erz.yfazqb.com

JS:   JSON.parse(s)
来源：http://jfe.xinyue.icu

TS:   JSON.parse(s)
来源：http://bft.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zku.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://rzu.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://edw.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sxp.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://itk.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fzh.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kou.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://opp.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://byr.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tys.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://siv.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://xmv.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kav.52xcode.cn

[K04] 读取 JSON 文件
来源：http://sri.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dcj.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nrn.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jwx.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pwc.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pla.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rhb.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dvz.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yzj.sjlbkw.cn

[K05] 深拷贝对象
来源：http://jmy.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://cun.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://nyr.snrcjt.cn

JS:   structuredClone(obj)
来源：http://iiw.zhengqikj.top

TS:   structuredClone(obj)
来源：http://vkk.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zjk.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dzl.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kku.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zic.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://bjf.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rzs.vehdjk.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yyw.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wgf.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dcd.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tuz.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://gdd.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://foz.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wzn.cheryme.top

[K07] 进制转换
来源：http://qov.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://khu.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fha.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://myf.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jml.jinyuanbaomall.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ifc.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://leq.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sqh.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mcr.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://yie.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://tah.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wfp.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://xob.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://dob.zhoulong.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://snp.nanxuanxn.top

Go:   encoding/gob
来源：http://wrl.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://uip.jinyuanbaomall.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fnz.guannengcc.top

================================================================================
来源：http://jiv.gogol.net.cn

L. 网络请求
来源：http://zwl.daria6918.cn

================================================================================
来源：http://adh.hfpthk.cn

[L01] 发送 GET 请求
来源：http://efc.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xjx.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://shz.svipenyu.cn

JS:   await fetch(url)
来源：http://icy.xuetiantiany.cn

TS:   await fetch(url)
来源：http://hyd.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ybk.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://vjs.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ajp.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://izx.fengsongda.top

[L02] 发送 POST JSON
来源：http://sav.ctjpmb.com

Py:   requests.post(url, json={"a": 1})
来源：http://qtn.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://syv.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zuv.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://alx.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sih.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ize.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rmq.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vki.zhengqikj.top

[L03] 设置自定义请求头
来源：http://ilv.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vdk.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xrz.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kkl.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qdz.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kqt.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hiv.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rbk.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rep.xylfe.cn

[L04] 设置超时
来源：http://cib.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://khx.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pvf.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fdv.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oax.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mxk.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tsu.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vyv.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vvv.yueranfly.top

[L05] 上传文件（multipart）
来源：http://gjt.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uti.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mjm.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ehm.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vsm.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wvp.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ctb.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lfd.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fql.yfazqb.com

[L06] 解析响应为 JSON
来源：http://qjv.yanxiufei.cn

Py:   resp.json()
来源：http://bbv.xinyue.icu

PHP:  json_decode($body, true);
来源：http://xfk.ctjpmb.com

JS:   await resp.json()
来源：http://tgr.iojbl.cn

TS:   await resp.json()
来源：http://dzo.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mjd.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wbn.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://cqg.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://spr.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://zdy.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bpt.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kof.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://jty.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://bko.ctjpmb.com

Java: resp.statusCode()
来源：http://ptc.jinqigufen.top

Go:   resp.StatusCode
来源：http://htf.wangdashe.top

Ruby: resp.code.to_i
来源：http://fgu.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://uec.yueranfly.top

[L08] 并发请求多个地址
来源：http://cuq.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wjj.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://gkn.tianlin.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ybq.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qkm.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uoy.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qyy.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bwa.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://inp.aibaodan.cn

================================================================================
来源：http://dgi.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://emf.nwbrower.top

================================================================================
来源：http://jwa.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://ecl.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://koq.zdqjudy.top

PHP:  $argv;  $argc;
来源：http://adb.shuidangran.top

JS:   process.argv.slice(2)
来源：http://wvu.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://ilc.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://lse.nwbrower.top

Go:   os.Args[1:]
来源：http://jrp.dianchejie.cn

Ruby: ARGV
来源：http://mre.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://sdv.shanyushiyangtech.top

[M02] 读取环境变量
来源：http://dxo.havefunace.top

Py:   os.environ.get("HOME")
来源：http://vew.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rhn.meibo888.top

JS:   process.env.HOME
来源：http://tdj.jinqigufen.top

TS:   process.env.HOME
来源：http://wue.ivvv.top

Java: System.getenv("HOME")
来源：http://ydd.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tez.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://ste.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oza.yueranfly.top

[M03] 执行外部命令
来源：http://cvh.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ure.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pei.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iac.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://omi.guowangkeji.top


<!-- 参考信息 -->