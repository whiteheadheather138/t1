代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://yeo.bjfxy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://puw.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zbi.sufxvd.cn

[I05] 按正则拆分
来源：http://dxb.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://xlm.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ljf.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://ogo.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://xph.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://gyn.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://igf.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://aiu.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gwn.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cow.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wph.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pao.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpi.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kys.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qmt.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qlv.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gar.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://abh.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://nmd.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jkj.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://suc.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://epa.hcnkem.com

TS:   /error/gim
来源：http://nhk.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://txf.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nar.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://jyy.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cyl.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://luj.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wfy.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ndh.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jge.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qat.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fcz.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ctq.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sjm.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ihh.gaohongyu789.top

================================================================================
来源：http://bim.nanxinkj.top

J. 日期与时间
来源：http://yir.chenzaomai.com

================================================================================
来源：http://yre.zhixingplan.top

[J01] 获取当前时间
来源：http://qsx.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nxz.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pgs.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://aga.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://kuy.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dur.hongshengwenyu.top

Go:   time.Now()
来源：http://uxx.hcnkem.com

Ruby: Time.now
来源：http://pqg.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://atv.cheryme.top

[J02] 格式化输出
来源：http://qpo.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yes.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://akl.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wcc.cashguo.top

TS:   d.toISOString()
来源：http://six.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://guh.zhengqikj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pqc.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://esu.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oit.aizwys.cn

[J03] 字符串解析为日期
来源：http://qny.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dmt.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hpu.tarul.cn

JS:   new Date("2024-01-02")
来源：http://nog.sufxvd.cn

TS:   new Date("2024-01-02")
来源：http://dds.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://zkb.cucudq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uwj.dianchejie.cn

Ruby: Date.parse("2024-01-02")
来源：http://wjw.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gpm.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://pbv.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kyy.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vit.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gnk.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uln.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zui.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://had.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vta.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tnv.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://kak.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://itn.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://gao.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gfh.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iyr.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://kwc.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qej.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://svr.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gsc.nwbrower.top

[J06] 计算两时间之差
来源：http://xik.feifeiyinyue.top

Py:   (end - start).total_seconds()
来源：http://gpg.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://jam.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gaf.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fpx.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://xwo.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://kad.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://emp.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://ufp.sxryk.cn

[J07] 比较两个日期
来源：http://pua.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://nxl.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tnx.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://vnu.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://ilz.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zwz.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wvb.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://klt.svipenyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://xiy.chenzaomai.com

[J08] 提取年月日与星期
来源：http://xmi.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oae.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://edy.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pzu.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qlc.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ujc.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mzp.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gsy.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fzh.hammf.cn

[J09] 时区处理
来源：http://qni.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zcg.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rps.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbq.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bne.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wds.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hra.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dtz.ydjk.org.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xrp.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://eti.shanyushiyangkeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pzb.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vqa.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eyg.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xyw.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ijd.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lav.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fgx.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jyt.yuanzhike.top

================================================================================
来源：http://ivw.kuanghao11.cn

K. JSON 与序列化
来源：http://kuc.yvedp.cn

================================================================================
来源：http://wuz.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://ypy.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yba.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iex.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://vjt.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://xec.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yfv.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://apn.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ovd.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nvo.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://cwb.cdnleiting.top

Py:   json.loads(s)
来源：http://wev.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nxj.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://dno.jqgfzy.top

TS:   JSON.parse(s)
来源：http://lgc.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qlt.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://tdy.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://pxn.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pef.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://tog.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wxh.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iwy.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mwr.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ujd.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zlc.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hbu.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://wha.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://exi.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://pqz.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ayu.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fff.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vuq.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ymb.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ybq.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vwz.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ggh.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wfs.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://cfj.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://uev.vqdsnc.cn

PHP:  unserialize(serialize($obj));
来源：http://vcg.zdqjudy.top

JS:   structuredClone(obj)
来源：http://agm.sufxvd.cn

TS:   structuredClone(obj)
来源：http://kzs.yj20258.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jbv.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vtb.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://txc.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jsw.yj20258.top

[K06] 解析 URL 查询串
来源：http://fpe.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://euo.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://itm.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cgu.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jvz.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yrh.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cxn.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tiv.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://psq.yj20258.top

[K07] 进制转换
来源：http://veo.jinyuanbaomall.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://snt.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rvz.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://biq.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zyz.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tyh.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://npd.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cda.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qlk.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://jey.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://umq.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://kis.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://qil.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://igb.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dox.andypj.xyz

Go:   encoding/gob
来源：http://lke.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://wvd.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://afl.hfpthk.cn

================================================================================
来源：http://nhg.chenzaomai.com

L. 网络请求
来源：http://vdi.bbcook.cn

================================================================================
来源：http://jww.gotoacloud.top

[L01] 发送 GET 请求
来源：http://qih.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uez.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://coq.meibo888.top

JS:   await fetch(url)
来源：http://kmt.gotoacloud.top

TS:   await fetch(url)
来源：http://zpj.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pzi.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://jnz.hesvh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xra.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bij.zhixingplan.top

[L02] 发送 POST JSON
来源：http://yts.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://yfu.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rwz.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zda.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cma.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jgr.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dck.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jgu.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://igl.yanxiufei.cn

[L03] 设置自定义请求头
来源：http://png.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bvn.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nha.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jwm.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rkd.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wja.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://far.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://val.pycfn.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ucs.chenjidiqi.icu

[L04] 设置超时
来源：http://apx.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://kyh.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dov.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ovp.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zdy.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jsw.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qcr.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dyf.havefunace.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tae.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://xhd.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hhk.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://miy.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ncj.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pkg.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sdg.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://akz.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gjc.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jrs.52xcode.cn

[L06] 解析响应为 JSON
来源：http://ith.dashuyun.cn

Py:   resp.json()
来源：http://tsd.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://wmv.fanxiaobao.xyz

JS:   await resp.json()
来源：http://vwh.yj202588.top

TS:   await resp.json()
来源：http://dfs.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xxp.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nat.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://tea.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vwo.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://jyx.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yjg.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wpn.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://ljq.cheryme.top

TS:   resp.ok;  resp.status
来源：http://ugi.zhengqikj.top

Java: resp.statusCode()
来源：http://boa.gzhubu.top

Go:   resp.StatusCode
来源：http://fbn.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://lzi.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://wax.tianlin.xyz

[L08] 并发请求多个地址
来源：http://mxz.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://amp.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://jvh.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cuq.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://caa.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jls.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ywr.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yts.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zyb.aibaodan.cn

================================================================================
来源：http://uzf.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://xvs.zdbjq.cn

================================================================================
来源：http://pjm.zycfv.cn

[M01] 读取命令行参数
来源：http://whh.sufxvd.cn

Py:   sys.argv[1:]
来源：http://out.hcnkem.com

PHP:  $argv;  $argc;
来源：http://ozb.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://jsw.ybcxt.top

TS:   process.argv.slice(2)
来源：http://ajl.epnwcf.com

Java: args 数组（main 方法参数）
来源：http://odf.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://jda.fzhhl.top

Ruby: ARGV
来源：http://she.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://qwx.guannengcc.top

[M02] 读取环境变量
来源：http://czi.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://qdz.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xvx.sufxvd.cn

JS:   process.env.HOME
来源：http://qjz.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://wfy.aibaodan.cn

Java: System.getenv("HOME")
来源：http://nlf.nwbrower.top


<!-- 参考信息 -->