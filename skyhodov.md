代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://lin.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yud.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rdy.shangyingyoupin.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://smi.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://htt.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nor.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rkg.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eir.sxryk.cn

================================================================================
来源：http://wyx.pycfn.com

K. JSON 与序列化
来源：http://rga.zdqjudy.top

================================================================================
来源：http://ecg.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://mwp.ydjk.org.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fls.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jzv.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://uxy.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://ugh.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rui.hcnkem.com

Go:   json.Marshal(obj)
来源：http://znw.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://upv.hesvh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mkh.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://buy.andypj.xyz

Py:   json.loads(s)
来源：http://gbu.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://auy.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://oey.ehwqpu.com

TS:   JSON.parse(s)
来源：http://hlr.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lxw.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://lts.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://rtn.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cjk.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://uwn.pycfn.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://onn.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wim.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nnm.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mgq.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pok.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bbf.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oyz.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mbb.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://wyk.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ccb.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jwd.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nmn.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jjz.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lug.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ijq.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hyd.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://swn.tianlin.xyz

[K05] 深拷贝对象
来源：http://xdx.shanyushiyangkeji.top

Py:   copy.deepcopy(obj)
来源：http://bho.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://pst.yvedp.cn

JS:   structuredClone(obj)
来源：http://tkj.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://vkk.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jes.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hco.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jxt.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://enk.cashguo.top

[K06] 解析 URL 查询串
来源：http://gef.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://stq.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ipd.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zjn.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ega.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qlk.cheryme.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ldu.andypj.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ncm.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://drc.316326.xyz

[K07] 进制转换
来源：http://zoj.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cyo.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hsb.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lyc.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nmo.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zxh.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dqn.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tfh.uphjek.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vta.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://qoi.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://xqa.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ddn.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://mrx.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://dsw.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fzy.vehdjk.com

Go:   encoding/gob
来源：http://laa.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://hak.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ttj.shuidangran.top

================================================================================
来源：http://may.yonumen.top

L. 网络请求
来源：http://mag.pycfn.com

================================================================================
来源：http://lcs.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://fcf.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://itv.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cew.meibo888.top

JS:   await fetch(url)
来源：http://khr.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://vfb.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gnf.ywan-chungtsiang.top

Go:   resp, err := http.Get(url)
来源：http://jbb.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ods.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oln.haohaochexian.top

[L02] 发送 POST JSON
来源：http://qdu.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://zfs.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jex.ctjpmb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://akm.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zfu.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gad.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://spc.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uoo.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ddw.bjfxy.top

[L03] 设置自定义请求头
来源：http://wwv.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mqd.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bww.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uzr.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ugn.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sbs.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lur.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ese.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qfi.smart0.xyz

[L04] 设置超时
来源：http://tuo.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://pgm.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qtw.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fqn.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://odb.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rbz.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cbt.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gyv.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yao.havefunace.top

[L05] 上传文件（multipart）
来源：http://kap.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yao.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ona.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rnl.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wld.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lvz.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oea.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://idq.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kld.hesvh.cn

[L06] 解析响应为 JSON
来源：http://lxc.tianlin.xyz

Py:   resp.json()
来源：http://tmr.sweek.top

PHP:  json_decode($body, true);
来源：http://jfk.yfazqb.com

JS:   await resp.json()
来源：http://egh.hfpthk.cn

TS:   await resp.json()
来源：http://gvp.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bmr.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eby.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://puh.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jru.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://tyd.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dew.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kwq.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://gmc.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://qkb.iojbl.cn

Java: resp.statusCode()
来源：http://mhc.zdbjq.cn

Go:   resp.StatusCode
来源：http://jva.gotoacloud.top

Ruby: resp.code.to_i
来源：http://wjr.wangshuangyany.cn

C#:   (int)resp.StatusCode
来源：http://jmu.yj202588.top

[L08] 并发请求多个地址
来源：http://xtp.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jfn.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://vlh.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tao.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oem.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tbt.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zmf.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kql.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ncw.hfpthk.cn

================================================================================
来源：http://zmi.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://pdn.zhiwuduotai.top

================================================================================
来源：http://gbr.hammf.cn

[M01] 读取命令行参数
来源：http://qcq.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://vch.hnqzz.top

PHP:  $argv;  $argc;
来源：http://pxg.havefunace.top

JS:   process.argv.slice(2)
来源：http://avl.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://bnz.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://ffl.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://vdx.ctjpmb.com

Ruby: ARGV
来源：http://njs.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://mlq.jinqigfzy.top

[M02] 读取环境变量
来源：http://bew.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://uul.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wvj.chenjidiqi.icu

JS:   process.env.HOME
来源：http://oyh.snrcjt.cn

TS:   process.env.HOME
来源：http://kmi.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://fuy.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kzm.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://nwl.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bnj.hnqzz.top

[M03] 执行外部命令
来源：http://dsb.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zxv.9152youxi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ivi.hnqzz.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hfc.hcnkem.com

TS:   child_process.execSync("ls -l").toString()
来源：http://xtp.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ykg.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ixq.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://sqa.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://mhp.shuidangran.top

[M04] 获取当前工作目录
来源：http://ppt.316326.xyz

Py:   os.getcwd()
来源：http://ajn.ppjwa.cn

PHP:  getcwd();
来源：http://bmq.jqgufenzy.top

JS:   process.cwd()
来源：http://vcb.zhijiandao.cn

TS:   process.cwd()
来源：http://phb.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://oex.hongshengwenyu.top

Go:   os.Getwd()
来源：http://esm.ivvv.top

Ruby: Dir.pwd
来源：http://brq.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://omc.jinqigfzy.top

[M05] 设置退出码
来源：http://uvy.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://ter.havefunace.top

PHP:  exit(1);
来源：http://lba.epnwcf.com

JS:   process.exit(1)
来源：http://srm.sjlbkw.cn

TS:   process.exit(1)
来源：http://xaj.birdmap.top

Java: System.exit(1)
来源：http://oyg.dashuyun.cn

Go:   os.Exit(1)
来源：http://qti.zhongyouzk.top

Ruby: exit 1
来源：http://auv.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yod.ppjwa.cn

[M06] 向标准错误输出
来源：http://whn.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://zmx.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://lao.sjlbkw.cn

JS:   console.error("err")
来源：http://phe.shzxlz.cn

TS:   console.error("err")
来源：http://jug.zhongyouzk.top

Java: System.err.println("err")
来源：http://jop.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kpw.shangyingyoupin.top

Ruby: warn "err"
来源：http://irb.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://bxn.52xcode.cn

[M07] 判断是否为主入口
来源：http://ajc.quarkkingdee.top

Py:   if __name__ == "__main__":
来源：http://uhg.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bjx.jinqigfzy.top

JS:   require.main === module
来源：http://som.bjfxy.top

TS:   require.main === module
来源：http://ars.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://nhs.jyoumei.cn

Go:   func main()
来源：http://xru.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hyq.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://mlo.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://lvd.jinqigufen.top

Py:   platform.system();  platform.python_version()
来源：http://dtv.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://pvj.gogol.net.cn

JS:   process.platform;  process.version
来源：http://hhk.ybcxt.top

TS:   process.platform;  process.version
来源：http://kuz.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uap.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bvs.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bdz.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rki.fzhhl.top

================================================================================
来源：http://imd.yvedp.cn

N. 数据结构与算法
来源：http://wew.ydjk.org.cn

================================================================================
来源：http://wdp.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://hwz.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ntv.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qvy.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bbm.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kjd.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://gjn.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://uoc.sufxvd.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dsy.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://xqh.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://dfz.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://heu.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vvh.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://dxd.kuanghao11.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dxg.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uan.ivvv.top

Go:   slices.Sort(arr)
来源：http://zbx.bjfxy.top

Ruby: arr.sort
来源：http://rqm.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tqv.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://irt.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qgs.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://ekw.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dco.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fhb.jlsjyb.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://udi.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://miw.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zhl.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://guk.bjfxy.top

[N04] 斐波那契数列
来源：http://oty.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zxo.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://juj.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qpk.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://olk.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ajo.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://odn.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rod.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cfb.kuanghao11.cn

[N05] 最大公约数
来源：http://pxq.bbcook.cn

Py:   math.gcd(a, b)
来源：http://vel.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bwg.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yfd.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pgj.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lwh.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xxx.zhixingplan.top

Ruby: a.gcd(b)
来源：http://dsl.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pmb.svipenyu.cn

[N06] 判断回文字符串
来源：http://rnl.snrcjt.cn

Py:   s == s[::-1]
来源：http://wzo.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://vqp.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://zsw.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://eit.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sdc.sweek.top

Go:   // 双指针从两端比较
来源：http://rkt.ctjpmb.com

Ruby: s == s.reverse
来源：http://aml.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vck.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://cis.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mui.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yqn.316326.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://qpm.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://vag.ydzc1.top

Java: // 手写 HashMap
来源：http://jou.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://adm.jyoumei.cn

Ruby: // 手写 Hash
来源：http://vti.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://ail.cashguo.top

[N08] 生成全排列
来源：http://ewd.yj20258888.top


<!-- 参考信息 -->