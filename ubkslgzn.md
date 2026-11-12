代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tot.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://szx.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xwh.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zhb.xziqi.cn

================================================================================
来源：http://wka.sufxvd.cn

K. JSON 与序列化
来源：http://fif.nanxinkj.top

================================================================================
来源：http://jat.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://dvv.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iwi.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qdv.sweek.top

JS:   JSON.stringify(obj)
来源：http://dij.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://sne.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lzm.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://sub.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://hpr.ybcxt.top

C#:   JsonSerializer.Serialize(obj)
来源：http://eqo.ctjpmb.com

[K02] JSON 字符串转对象
来源：http://nsx.shangyingyoupin.top

Py:   json.loads(s)
来源：http://umc.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://brr.cdnleiting.top

JS:   JSON.parse(s)
来源：http://dsl.bjfxy.top

TS:   JSON.parse(s)
来源：http://ibr.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ise.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://kus.xinyue.icu

Ruby: JSON.parse(s)
来源：http://hcn.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://szg.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://fyd.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oqo.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cdc.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hve.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gew.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mlp.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://shm.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://xov.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://esj.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://ruv.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pzu.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pyh.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://umd.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oga.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kvg.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://juj.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rng.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://coy.jlsjyb.cn

[K05] 深拷贝对象
来源：http://ruw.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://sbu.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://tnz.zhixingplan.top

JS:   structuredClone(obj)
来源：http://pfe.ydzc1.top

TS:   structuredClone(obj)
来源：http://eex.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ipg.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lii.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xlx.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xxi.sweek.top

[K06] 解析 URL 查询串
来源：http://ido.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hia.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lkx.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zfk.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sab.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hty.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dep.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://egk.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tag.gogol.net.cn

[K07] 进制转换
来源：http://xim.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rdc.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mgu.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jyc.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sav.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rlo.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qbj.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rvs.nanxinkj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ipp.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://ljs.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://cxs.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tco.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://dyb.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://nwp.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ysg.daria6918.cn

Go:   encoding/gob
来源：http://gvq.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://hng.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hyy.52xcode.cn

================================================================================
来源：http://kkw.ehwqpu.com

L. 网络请求
来源：http://puy.zdbjq.cn

================================================================================
来源：http://wai.xuanzx.com

[L01] 发送 GET 请求
来源：http://jcl.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jwx.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hmt.sweek.top

JS:   await fetch(url)
来源：http://ydx.hywenlv.cn

TS:   await fetch(url)
来源：http://mbo.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://atu.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://ozd.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hfn.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mte.jinqigufen.top

[L02] 发送 POST JSON
来源：http://eyq.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xuc.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bkj.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wmw.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jne.meibo888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jcm.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jad.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dsr.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ugp.svipenyu.cn

[L03] 设置自定义请求头
来源：http://sqb.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hvr.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iec.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uzv.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pnq.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ogq.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wnr.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://drn.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yuw.zhixingplan.top

[L04] 设置超时
来源：http://nad.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://fri.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jye.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gxt.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ftw.kuanghao11.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wma.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lsk.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ohu.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ahg.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://zah.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pdd.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ald.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mei.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pae.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jvw.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxj.smart0.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qlb.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cgg.xuanzx.com

[L06] 解析响应为 JSON
来源：http://itr.andypj.xyz

Py:   resp.json()
来源：http://ane.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://chv.daxiang520.top

JS:   await resp.json()
来源：http://yau.yj202588.top

TS:   await resp.json()
来源：http://wzo.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ltp.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nor.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://osb.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ari.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://ixe.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ebh.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aec.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://xgb.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://dtk.hongshengwenyu.top

Java: resp.statusCode()
来源：http://uke.wangdashe.top

Go:   resp.StatusCode
来源：http://tek.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://eae.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://lgz.aizwys.cn

[L08] 并发请求多个地址
来源：http://ipv.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rnf.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://mvr.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dql.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bug.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yuq.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zim.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pqc.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jlj.haohaochexian.top

================================================================================
来源：http://zkw.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://gmv.gotoacloud.top

================================================================================
来源：http://uzd.gaohongyu789.top

[M01] 读取命令行参数
来源：http://cjl.zycfv.cn

Py:   sys.argv[1:]
来源：http://kdr.redwolf501.top

PHP:  $argv;  $argc;
来源：http://lbo.sweek.top

JS:   process.argv.slice(2)
来源：http://jrq.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://yif.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://jjb.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://kbv.birdmap.top

Ruby: ARGV
来源：http://tiy.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://gki.shangyingyoupin.top

[M02] 读取环境变量
来源：http://tnl.316326.xyz

Py:   os.environ.get("HOME")
来源：http://pwn.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zow.tianlin.xyz

JS:   process.env.HOME
来源：http://cyn.ppjwa.cn

TS:   process.env.HOME
来源：http://aka.gotoacloud.top

Java: System.getenv("HOME")
来源：http://rpq.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jps.fzhhl.top

Ruby: ENV["HOME"]
来源：http://ase.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://quf.dianchejie.cn

[M03] 执行外部命令
来源：http://cib.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://haf.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iti.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://iok.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bgh.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://enn.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zmq.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bok.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://gar.mhx1999.top

[M04] 获取当前工作目录
来源：http://uui.shangyingyoupin.top

Py:   os.getcwd()
来源：http://hfr.tianlin.xyz

PHP:  getcwd();
来源：http://ywc.quarkkingdee.top

JS:   process.cwd()
来源：http://zhg.mhx1999.top

TS:   process.cwd()
来源：http://jzv.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://rqc.9152youxi.cn

Go:   os.Getwd()
来源：http://dco.dianchejie.cn

Ruby: Dir.pwd
来源：http://vvr.feifeiyinyue.top

C#:   Directory.GetCurrentDirectory()
来源：http://xrp.tarul.cn

[M05] 设置退出码
来源：http://owo.bjfxy.top

Py:   sys.exit(1)
来源：http://hav.yuanzhike.top

PHP:  exit(1);
来源：http://wmb.gogol.net.cn

JS:   process.exit(1)
来源：http://lgl.xuetiantiany.cn

TS:   process.exit(1)
来源：http://apb.meibo888.top

Java: System.exit(1)
来源：http://dqo.gzhubu.top

Go:   os.Exit(1)
来源：http://jwg.hcnkem.com

Ruby: exit 1
来源：http://cqm.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aqw.svipenyu.cn

[M06] 向标准错误输出
来源：http://cjm.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://seb.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uij.yangfankeji.com

JS:   console.error("err")
来源：http://zpd.chenjidiqi.icu

TS:   console.error("err")
来源：http://fte.snrcjt.cn

Java: System.err.println("err")
来源：http://ypb.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://txa.wangshuangyany.cn

Ruby: warn "err"
来源：http://nzl.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://srt.shuidangran.top

[M07] 判断是否为主入口
来源：http://vfd.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://mdh.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gyv.jqgfzy.top

JS:   require.main === module
来源：http://lmq.nwbrower.top

TS:   require.main === module
来源：http://quw.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://rmh.sweek.top

Go:   func main()
来源：http://vam.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zxt.hesvh.cn

C#:   static void Main(string[] args)
来源：http://jdu.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://veb.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://fqk.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://vrw.ctjpmb.com

JS:   process.platform;  process.version
来源：http://xfs.hcnkem.com

TS:   process.platform;  process.version
来源：http://rop.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sny.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dab.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xgb.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://snj.yuanzhike.top

================================================================================
来源：http://gsb.yangfankeji.com

N. 数据结构与算法
来源：http://nmn.nanxinkj.top

================================================================================
来源：http://ede.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://dru.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bht.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kkp.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kpy.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xpq.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://nvi.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://lup.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://zce.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://uhr.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://kae.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://xcr.ehwqpu.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kfj.bbcook.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vcn.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jym.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lkm.sjlbkw.cn

Go:   slices.Sort(arr)
来源：http://wlb.iojbl.cn

Ruby: arr.sort
来源：http://zak.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ita.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://tqo.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rly.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://emt.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sss.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pbn.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hzf.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://red.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zps.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://qdx.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://jis.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://njy.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ftm.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://irt.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cvc.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tde.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tmn.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xfj.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://voo.cdnleiting.top

[N05] 最大公约数
来源：http://wyg.fengsongda.top

Py:   math.gcd(a, b)
来源：http://bvq.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://epe.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wrr.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dws.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pwb.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ggx.chenzaomai.com

Ruby: a.gcd(b)
来源：http://rff.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ahz.nwbrower.top

[N06] 判断回文字符串
来源：http://feb.daxiang520.top

Py:   s == s[::-1]
来源：http://bsd.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://toc.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://ama.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://rzt.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nqn.yuxming.cn

Go:   // 双指针从两端比较
来源：http://rxo.pycfn.com

Ruby: s == s.reverse
来源：http://paq.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dqb.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://ksp.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ffx.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mec.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qre.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://tkv.jinqigfzy.top

Java: // 手写 HashMap
来源：http://ymd.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://rqx.birdmap.top

Ruby: // 手写 Hash
来源：http://kzz.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://usa.epnwcf.com

[N08] 生成全排列
来源：http://bic.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://yzn.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://onb.yfazqb.com

JS:   // 手写回溯递归
来源：http://xmg.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://cso.zycfv.cn


<!-- 参考信息 -->