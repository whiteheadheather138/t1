代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://yjs.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lca.ctjpmb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rfs.c1oappe.top

[I05] 按正则拆分
来源：http://rkg.c1oappe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ibi.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rmk.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://rmp.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://ygp.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://pmv.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uat.tanke756.top

Ruby: s.split(/\s*,\s*/)
来源：http://dkq.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://axw.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hgw.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ftw.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://duy.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tqo.cqqwz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ogf.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://npa.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pzh.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kbj.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://atz.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://whi.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rnu.jinqigufen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kvv.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nig.yj20258.top

TS:   /error/gim
来源：http://lzo.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ill.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cna.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://vyp.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://std.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://isa.hcnkem.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pvd.smart0.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://buv.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://awq.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://omk.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://zwh.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xte.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ufp.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ixm.c1oappe.top

================================================================================
来源：http://cbn.jinqigufen.top

J. 日期与时间
来源：http://yhq.xinyue.icu

================================================================================
来源：http://ngp.haohaochexian.top

[J01] 获取当前时间
来源：http://xjc.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://iur.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nhz.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://bqq.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://ywo.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zff.sweek.top

Go:   time.Now()
来源：http://ths.fehbvm.com

Ruby: Time.now
来源：http://zxw.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eew.daria6918.cn

[J02] 格式化输出
来源：http://sni.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qkt.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qxm.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lhw.zhiwuduotai.top

TS:   d.toISOString()
来源：http://kce.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://toc.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ttm.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hju.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xpo.fehbvm.com

[J03] 字符串解析为日期
来源：http://mtt.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ahy.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uop.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://hfh.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://vvc.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://wat.guowangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tlb.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://wgk.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gmq.sweek.top

[J04] 时间戳与日期互转
来源：http://zxf.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wyw.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xfp.quarkkingdee.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hiq.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://elw.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uoe.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bwt.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vso.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://umv.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://yts.ivvv.top

Py:   now + timedelta(days=7)
来源：http://fom.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ndy.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nga.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rgp.xingfuxueyuan.xyz

Java: LocalDate.now().plusDays(7)
来源：http://ifl.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://loe.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://eig.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://mzc.hesvh.cn

[J06] 计算两时间之差
来源：http://rlt.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://qna.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://ego.svipenyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://izt.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://frw.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://qrd.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://wcg.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://idx.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://elf.haohaochexian.top

[J07] 比较两个日期
来源：http://cwm.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://cxq.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cwg.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://tzs.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iba.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cnd.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wpi.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://ohl.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://qkn.shzxlz.cn

[J08] 提取年月日与星期
来源：http://xyp.xuetiantiany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pil.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://taq.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rqd.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aee.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://opn.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rte.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dyk.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ybh.shuidangran.top

[J09] 时区处理
来源：http://rpk.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dje.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xop.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mnv.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nsh.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qhd.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wqd.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gkw.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ura.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://gsb.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vdo.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hkv.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eey.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cck.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gep.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gvt.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wgn.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lhb.jinqigfzy.top

================================================================================
来源：http://njd.yuxming.cn

K. JSON 与序列化
来源：http://ycq.uphjek.com

================================================================================
来源：http://ntd.smart0.xyz

[K01] 对象转 JSON 字符串
来源：http://lsc.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://atb.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://trl.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://zam.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://ocl.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vqd.hesvh.cn

Go:   json.Marshal(obj)
来源：http://wti.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://lab.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gnn.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://lsb.pengpengdd.cyou

Py:   json.loads(s)
来源：http://tuu.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gdd.gogol.net.cn

JS:   JSON.parse(s)
来源：http://mbs.cqqwz.cn

TS:   JSON.parse(s)
来源：http://adf.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hln.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://kqv.tanke756.top

Ruby: JSON.parse(s)
来源：http://fzm.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eia.shuidangran.top

[K03] JSON 美化输出（带缩进）
来源：http://gzp.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kyi.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dib.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hvw.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://efx.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ara.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://quj.wangdashe.top

Ruby: JSON.pretty_generate(obj)
来源：http://ukk.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://giw.jianghu66.top

[K04] 读取 JSON 文件
来源：http://ayk.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dil.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iki.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yyq.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dxn.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://opp.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wbf.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gpt.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dbv.shzxlz.cn

[K05] 深拷贝对象
来源：http://jgt.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://ptz.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://ylb.daxiang520.top

JS:   structuredClone(obj)
来源：http://jwi.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://geo.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bfu.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bwi.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fwo.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yvd.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://ubq.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://api.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jbf.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kwu.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ala.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://elc.iojbl.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tfg.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ndt.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vdh.xziqi.cn

[K07] 进制转换
来源：http://rmh.yfazqb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nzr.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pzy.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zuz.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uwl.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oph.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vmc.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pwh.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xox.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://aui.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://ojv.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mhg.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://dea.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://yrd.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ttn.daria6918.cn

Go:   encoding/gob
来源：http://hrb.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://jwx.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sak.zdqjudy.top

================================================================================
来源：http://mis.ywan-chungtsiang.top

L. 网络请求
来源：http://swf.jqgufenzy.top

================================================================================
来源：http://pxy.yvedp.cn

[L01] 发送 GET 请求
来源：http://wwy.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xqh.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fau.epnwcf.com

JS:   await fetch(url)
来源：http://dbe.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://yqx.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cbh.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://cgu.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://egs.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://deh.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://msw.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://icw.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rdx.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eoi.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ueg.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wtm.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mkb.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ufw.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://frk.bbcook.cn

[L03] 设置自定义请求头
来源：http://szf.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ufh.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dcl.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://enk.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xah.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ydm.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jrn.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ufd.chenjidiqi.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cuf.xuanzx.com

[L04] 设置超时
来源：http://jzv.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://tqs.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tbz.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bdh.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jef.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tsy.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kwr.xingfuxueyuan.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yrv.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gzw.bbcook.cn

[L05] 上传文件（multipart）
来源：http://joa.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://urm.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eye.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nhe.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xxg.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bro.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ecc.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cyw.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bex.tarul.cn

[L06] 解析响应为 JSON
来源：http://abf.jinqigfzy.top

Py:   resp.json()
来源：http://rht.aizwys.cn

PHP:  json_decode($body, true);
来源：http://rga.hammf.cn

JS:   await resp.json()
来源：http://jou.xylfe.cn

TS:   await resp.json()
来源：http://nvj.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lhf.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pvz.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://gyt.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://otn.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://ggx.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mqr.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ajb.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://rmo.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://wzs.cqqwz.cn

Java: resp.statusCode()
来源：http://gjo.daria6918.cn

Go:   resp.StatusCode
来源：http://tjb.epnwcf.com

Ruby: resp.code.to_i
来源：http://xkt.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://snb.tianlin.xyz

[L08] 并发请求多个地址
来源：http://dcq.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ksk.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://qsi.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://edk.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dzw.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://igs.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jun.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bsd.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yee.hywenlv.cn

================================================================================
来源：http://nua.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://orf.chenzaomai.com

================================================================================
来源：http://uqo.yj20258.top

[M01] 读取命令行参数
来源：http://yde.ydzc1.top

Py:   sys.argv[1:]
来源：http://ark.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://dge.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://tqh.mhx1999.top

TS:   process.argv.slice(2)
来源：http://qhh.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://baf.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://ijv.meibo888.top

Ruby: ARGV
来源：http://wqs.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://zlr.tarul.cn

[M02] 读取环境变量
来源：http://uxs.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://zri.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pqt.aizwys.cn

JS:   process.env.HOME
来源：http://mmx.zycfv.cn

TS:   process.env.HOME
来源：http://foh.ctjpmb.com

Java: System.getenv("HOME")
来源：http://xcr.xuetiantiany.cn


<!-- 参考信息 -->