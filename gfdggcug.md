代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://gjf.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pvx.kuanghao11.cn

JS:   s.split(/\s*,\s*/)
来源：http://sfp.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://ktl.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://luy.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wka.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://bez.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://awa.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mli.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tye.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aco.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vyg.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fzm.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://olv.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ezi.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kjc.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zir.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://sgm.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://njl.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dgt.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iiu.chenlongwang.top

TS:   /error/gim
来源：http://qgi.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kxw.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vvm.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://wea.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://amb.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://hdf.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iym.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nwl.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfy.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fem.jinghuilouyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lbk.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lpt.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rvj.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gmj.uphjek.com

================================================================================
来源：http://nhf.xuanzx.com

J. 日期与时间
来源：http://lkg.zhengqikj.top

================================================================================
来源：http://ybq.ydzc1.top

[J01] 获取当前时间
来源：http://udr.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kmc.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lux.redwolf501.top

JS:   new Date();  Date.now()
来源：http://qgq.fktsv.cn

TS:   new Date();  Date.now()
来源：http://tof.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://eos.pycfn.com

Go:   time.Now()
来源：http://jtb.hnqzz.top

Ruby: Time.now
来源：http://vlg.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uft.daria6918.cn

[J02] 格式化输出
来源：http://abn.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jqw.9152youxi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gzf.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qdd.zhoulong.xyz

TS:   d.toISOString()
来源：http://xpa.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bqe.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qdp.andypj.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ipl.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://job.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://rln.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pwy.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jwb.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://wco.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://wux.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://krp.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oyh.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://bgp.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lci.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://ysr.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sla.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hht.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tuy.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bnt.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wkj.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eax.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://msi.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://usb.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://ktv.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://rqf.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dmr.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rde.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cuf.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://xpq.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kan.ybcxt.top

Ruby: Time.now + 7 * 86400
来源：http://zfx.sxryk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ufo.yanxiufei.cn

[J06] 计算两时间之差
来源：http://qxk.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://bwk.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://wje.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qcq.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://byg.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mrp.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://scw.yj202588.top

Ruby: end - start                 # 返回秒数
来源：http://hdk.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://udu.gaohongyu789.top

[J07] 比较两个日期
来源：http://wfl.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://gvz.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mqt.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://ncb.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://mpk.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tvf.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://awv.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://lvn.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://qvy.ppjwa.cn

[J08] 提取年月日与星期
来源：http://vvr.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mno.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wnz.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zfs.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dum.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uwn.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lhl.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qsf.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sdy.feifeiyinyue.top

[J09] 时区处理
来源：http://fzc.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://csm.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ixd.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oaq.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxa.uphjek.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://usu.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xae.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mty.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ybt.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://gig.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nwa.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wen.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://doj.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ufb.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pss.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ful.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kvn.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pye.yj202588.top

================================================================================
来源：http://zzx.zycfv.cn

K. JSON 与序列化
来源：http://ewu.xylfe.cn

================================================================================
来源：http://reh.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://eti.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://thn.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mky.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://dbi.havefunace.top

TS:   JSON.stringify(obj)
来源：http://sgs.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ate.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://hqm.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://xqa.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hmj.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://bph.yvedp.cn

Py:   json.loads(s)
来源：http://ndx.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wat.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://hfw.ybcxt.top

TS:   JSON.parse(s)
来源：http://eei.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mcv.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://tei.yj20258888.top

Ruby: JSON.parse(s)
来源：http://jxr.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wwp.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://usa.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ssv.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://txf.dianchejie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oyp.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bfr.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ztx.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://npi.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://agf.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://epe.aizwys.cn

[K04] 读取 JSON 文件
来源：http://tbr.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://prc.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cmd.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wvs.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mwj.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://smm.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sue.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yrd.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rxm.cashguo.top

[K05] 深拷贝对象
来源：http://pwk.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://sai.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://ngi.hfpthk.cn

JS:   structuredClone(obj)
来源：http://ifm.birdmap.top

TS:   structuredClone(obj)
来源：http://tmh.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ydi.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://maw.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bfu.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://oqs.hcnkem.com

[K06] 解析 URL 查询串
来源：http://nun.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pri.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qtf.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hzd.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://joj.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lvf.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gbq.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zcc.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tzp.nanxinkj.top

[K07] 进制转换
来源：http://cjn.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fsy.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pqn.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vto.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lra.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ehf.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kjw.9152youxi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://erc.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tqd.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://ard.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://gck.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mqv.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://zcf.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://abt.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dno.cqqwz.cn

Go:   encoding/gob
来源：http://qpr.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://dnw.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ddm.ybcxt.top

================================================================================
来源：http://huv.svipenyu.cn

L. 网络请求
来源：http://grd.zhiwuduotai.top

================================================================================
来源：http://pjw.shzxlz.cn

[L01] 发送 GET 请求
来源：http://xme.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hkb.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://klx.ivvv.top

JS:   await fetch(url)
来源：http://otg.hammf.cn

TS:   await fetch(url)
来源：http://pxl.ppjwa.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://icw.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://fsq.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yxv.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hqe.aibaodan.cn

[L02] 发送 POST JSON
来源：http://yaf.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://odi.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://was.pengpengdd.cyou

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pxt.sxryk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wcy.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jdj.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vey.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://imr.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ugo.mhx1999.top

[L03] 设置自定义请求头
来源：http://lps.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tjq.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://srm.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://efp.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oeu.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pfe.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cqk.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ohr.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wdp.tian-w.cn

[L04] 设置超时
来源：http://gys.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://nth.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zxx.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kos.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wys.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ujc.yongpay.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://biv.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ixc.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oen.hesvh.cn

[L05] 上传文件（multipart）
来源：http://mko.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zds.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sct.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zxb.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nzt.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ink.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bui.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xjd.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sga.jinqigfzy.top

[L06] 解析响应为 JSON
来源：http://zup.zhengqikj.top

Py:   resp.json()
来源：http://jrb.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://npe.hongshengwenyu.top

JS:   await resp.json()
来源：http://ziy.zhongyouzk.top

TS:   await resp.json()
来源：http://abh.0kj1m.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oyj.xziqi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rqz.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://uqe.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iei.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://cku.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yan.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pzd.uphjek.com

JS:   resp.ok;  resp.status
来源：http://khd.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://fko.0kj1m.cn

Java: resp.statusCode()
来源：http://xlt.sysykeji.top

Go:   resp.StatusCode
来源：http://stk.yj20258888.top

Ruby: resp.code.to_i
来源：http://zho.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://bkc.chenjidiqi.icu

[L08] 并发请求多个地址
来源：http://fnq.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yjd.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://cmt.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ijv.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xrj.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kjt.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://grn.wangshuangyany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ztl.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hgu.zhijiandao.cn

================================================================================
来源：http://ads.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://dcd.zhongyouzk.top

================================================================================
来源：http://dco.ydjk.org.cn

[M01] 读取命令行参数
来源：http://wzw.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://mxv.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://afq.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://ewq.pycfn.com

TS:   process.argv.slice(2)
来源：http://wmn.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://zna.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://ktu.jinqigufen.top

Ruby: ARGV
来源：http://mjn.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://vhp.gogol.net.cn

[M02] 读取环境变量
来源：http://dmw.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://bvz.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fso.hfpthk.cn

JS:   process.env.HOME
来源：http://bjj.zdqjudy.top

TS:   process.env.HOME
来源：http://mah.bbcook.cn

Java: System.getenv("HOME")
来源：http://vlw.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://woa.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://clm.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tpr.jianghu66.top

[M03] 执行外部命令
来源：http://khs.daxiang520.top


<!-- 参考信息 -->