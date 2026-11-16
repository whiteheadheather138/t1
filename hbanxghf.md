代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://rfy.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jrc.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bkj.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aja.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zhf.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://leh.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bxs.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dmd.zdbjq.cn

================================================================================
来源：http://ucx.tianlin.xyz

K. JSON 与序列化
来源：http://yob.meibo888.top

================================================================================
来源：http://hle.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://osm.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dic.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xdh.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://jzj.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://eoq.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bkr.hnqzz.top

Go:   json.Marshal(obj)
来源：http://jbw.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://zpl.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ccx.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://ytl.shangyingyoupin.top

Py:   json.loads(s)
来源：http://zsg.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://too.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://fjy.ehwqpu.com

TS:   JSON.parse(s)
来源：http://hdo.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fcm.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://ank.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://doi.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://onb.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://iul.zdbjq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fpj.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ecf.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zgj.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fkq.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://onr.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://anw.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://vnt.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lzs.xuanzx.com

[K04] 读取 JSON 文件
来源：http://epm.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://swu.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tkc.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vhc.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uce.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://veg.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wxw.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bbq.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ssn.nwbrower.top

[K05] 深拷贝对象
来源：http://eyg.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://vnh.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://uge.hammf.cn

JS:   structuredClone(obj)
来源：http://igs.sysykeji.top

TS:   structuredClone(obj)
来源：http://ygy.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ypr.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sdj.jinqigufen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://azd.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oms.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://umc.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vua.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://atk.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dqy.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bqu.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nja.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ush.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://prt.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://atk.hywenlv.cn

[K07] 进制转换
来源：http://nex.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://crh.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pko.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qxp.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zux.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nbv.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fxr.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://efs.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mmp.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://agu.havefunace.top

Py:   pickle.dumps(obj)
来源：http://raf.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://etb.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://vtz.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://iqu.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iqn.jyoumei.cn

Go:   encoding/gob
来源：http://war.gzhubu.top

Ruby: Marshal.dump(obj)
来源：http://wdr.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hkv.ppjwa.cn

================================================================================
来源：http://mrz.yvedp.cn

L. 网络请求
来源：http://ace.aizwys.cn

================================================================================
来源：http://oqv.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://ihl.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kch.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gdg.sweek.top

JS:   await fetch(url)
来源：http://oib.dianchejie.cn

TS:   await fetch(url)
来源：http://oxu.hywenlv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yoa.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://eef.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://okb.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fuf.andypj.xyz

[L02] 发送 POST JSON
来源：http://sqf.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nan.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yzb.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lhs.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://csm.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lrs.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://isu.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://spl.jinyuanbaomall.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rgv.sweek.top

[L03] 设置自定义请求头
来源：http://jil.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kax.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ttj.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bnr.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wby.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mmt.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bbd.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wty.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ggs.sufxvd.cn

[L04] 设置超时
来源：http://eji.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://grt.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://izj.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wrn.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uki.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cxv.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rgt.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tfy.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ihj.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://zxu.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zuh.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qfz.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jfb.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wwg.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qoc.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://plx.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://djp.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://knj.yvedp.cn

[L06] 解析响应为 JSON
来源：http://ykf.jlsjyb.cn

Py:   resp.json()
来源：http://zvf.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://wwm.yongpay.top

JS:   await resp.json()
来源：http://bfx.guowangkeji.top

TS:   await resp.json()
来源：http://lca.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kgl.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://squ.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://jpz.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ohw.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://plt.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bnn.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xbg.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://nht.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://prr.0kj1m.cn

Java: resp.statusCode()
来源：http://rrb.guowangkeji.top

Go:   resp.StatusCode
来源：http://ncu.sufxvd.cn

Ruby: resp.code.to_i
来源：http://fln.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://dce.zdqjudy.top

[L08] 并发请求多个地址
来源：http://mml.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gye.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://dgs.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zbf.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xnm.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eyf.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lxd.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zia.vqdsnc.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vtr.sufxvd.cn

================================================================================
来源：http://dme.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://mfr.hesvh.cn

================================================================================
来源：http://nkl.hcnkem.com

[M01] 读取命令行参数
来源：http://hyo.tanke756.top

Py:   sys.argv[1:]
来源：http://qgf.hammf.cn

PHP:  $argv;  $argc;
来源：http://nrz.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://oxd.pycfn.com

TS:   process.argv.slice(2)
来源：http://lzh.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://fft.tanke756.top

Go:   os.Args[1:]
来源：http://yfs.gzhubu.top

Ruby: ARGV
来源：http://zvj.hnxiangtu.top

C#:   args 数组（Main 方法参数）
来源：http://obo.yfazqb.com

[M02] 读取环境变量
来源：http://iqh.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://vxc.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://chp.aizwys.cn

JS:   process.env.HOME
来源：http://ahd.redwolf501.top

TS:   process.env.HOME
来源：http://znb.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://vuh.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xit.yonumen.top

Ruby: ENV["HOME"]
来源：http://icl.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qre.nanxuanxn.top

[M03] 执行外部命令
来源：http://xny.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yqn.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wsp.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ilj.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://unj.vehdjk.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://svp.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://val.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://fnb.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://rzp.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://uft.chenlongwang.top

Py:   os.getcwd()
来源：http://kok.316326.xyz

PHP:  getcwd();
来源：http://svm.chenjidiqi.icu

JS:   process.cwd()
来源：http://kwx.hfpthk.cn

TS:   process.cwd()
来源：http://wfj.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://oqx.zhijiandao.cn

Go:   os.Getwd()
来源：http://xpn.tanke756.top

Ruby: Dir.pwd
来源：http://tdb.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://gtw.cucudq.cn

[M05] 设置退出码
来源：http://btk.fktsv.cn

Py:   sys.exit(1)
来源：http://agr.bbcook.cn

PHP:  exit(1);
来源：http://eqe.cashguo.top

JS:   process.exit(1)
来源：http://stc.zycfv.cn

TS:   process.exit(1)
来源：http://boa.birdmap.top

Java: System.exit(1)
来源：http://pbx.svipenyu.cn

Go:   os.Exit(1)
来源：http://uuk.ybcxt.top

Ruby: exit 1
来源：http://lbl.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cxj.hnqzz.top

[M06] 向标准错误输出
来源：http://ciw.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://xhy.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://oqe.xziqi.cn

JS:   console.error("err")
来源：http://xov.yueranfly.top

TS:   console.error("err")
来源：http://chl.zhengqikj.top

Java: System.err.println("err")
来源：http://bda.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vvn.yueranfly.top

Ruby: warn "err"
来源：http://fqf.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://eap.zdbjq.cn

[M07] 判断是否为主入口
来源：http://yym.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://pxv.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jlt.nwbrower.top

JS:   require.main === module
来源：http://kyj.fzhhl.top

TS:   require.main === module
来源：http://nkx.shuidangran.top

Java: public static void main(String[] args)
来源：http://uxr.jqgfzy.top

Go:   func main()
来源：http://try.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gzl.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://mfg.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://wyb.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://req.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://wnu.hcnkem.com

JS:   process.platform;  process.version
来源：http://jsq.yfazqb.com

TS:   process.platform;  process.version
来源：http://iap.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cgg.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gpe.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://btd.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://nkc.xingfuxueyuan.xyz

================================================================================
来源：http://rir.hnxiangtu.top

N. 数据结构与算法
来源：http://vuq.yfazqb.com

================================================================================
来源：http://qsd.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://fjq.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ogg.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://snx.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sfu.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://azz.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://buk.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://juq.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nwp.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zas.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://wvh.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://fwq.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tpx.meibo888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rlx.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hyf.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ebv.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://cdc.xuanzx.com

Ruby: arr.sort
来源：http://eog.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pwi.zhixingplan.top

[N03] 快速排序（分治示例）
来源：http://cia.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cad.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://ysp.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mmk.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uru.cucudq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://opu.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fdm.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hgr.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://unf.52xcode.cn

[N04] 斐波那契数列
来源：http://alh.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dcm.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ttm.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://znm.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cjf.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yzi.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gqw.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wun.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ldr.hfpthk.cn

[N05] 最大公约数
来源：http://ivh.yj20258.top

Py:   math.gcd(a, b)
来源：http://uaw.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fvh.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ojv.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yti.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rma.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gvl.sxryk.cn

Ruby: a.gcd(b)
来源：http://hqd.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ibd.fktsv.cn

[N06] 判断回文字符串
来源：http://vru.gzhubu.top

Py:   s == s[::-1]
来源：http://gcx.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://lfz.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://rjq.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://cny.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dte.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://kwr.zycfv.cn

Ruby: s == s.reverse
来源：http://dve.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eru.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://aue.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jlh.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://esu.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://llo.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://dtd.redwolf501.top

Java: // 手写 HashMap
来源：http://twd.smart0.xyz

Go:   // 手写 map[int]int
来源：http://dap.nanxinkj.top

Ruby: // 手写 Hash
来源：http://umz.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://yfy.xuetiantiany.cn

[N08] 生成全排列
来源：http://iwn.hcnkem.com


<!-- 参考信息 -->