代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rza.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sda.pycfn.com

JS:   JSON.stringify(obj)
来源：http://weg.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://dcd.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://osx.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://quq.svipenyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://blz.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://gbg.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://loc.cqqwz.cn

Py:   json.loads(s)
来源：http://pcp.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://czr.yuanzhike.top

JS:   JSON.parse(s)
来源：http://mos.bbcook.cn

TS:   JSON.parse(s)
来源：http://kse.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vej.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://qrb.ivvv.top

Ruby: JSON.parse(s)
来源：http://pbs.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ibn.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://oqb.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://umr.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://svv.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://fpn.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yni.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vxk.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://stz.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://rub.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yra.shuidangran.top

[K04] 读取 JSON 文件
来源：http://vyw.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bah.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://duh.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oit.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://twq.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://phl.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oue.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tya.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tpe.meibo888.top

[K05] 深拷贝对象
来源：http://qwr.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://orn.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://hdj.fehbvm.com

JS:   structuredClone(obj)
来源：http://ddb.yj202588.top

TS:   structuredClone(obj)
来源：http://pgf.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zfs.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zbd.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pro.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wqm.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://eif.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dyj.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bxi.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vfs.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hmj.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tpw.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wln.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tup.zhengqikj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bja.xinyue.icu

[K07] 进制转换
来源：http://aey.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mxu.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zib.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://afs.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lja.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kjt.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ptr.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pkx.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kpb.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://igi.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://xgd.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lit.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://qfw.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://ygy.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kvp.yanxiufei.cn

Go:   encoding/gob
来源：http://klc.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://cki.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ztr.chenlongwang.top

================================================================================
来源：http://xsb.zhaomingkeji.xyz

L. 网络请求
来源：http://ufa.sweek.top

================================================================================
来源：http://pgd.jiagoushi.top

[L01] 发送 GET 请求
来源：http://yez.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lgb.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lma.gotoacloud.top

JS:   await fetch(url)
来源：http://iys.jianghu66.top

TS:   await fetch(url)
来源：http://gam.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kqp.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://npp.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dvf.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qkd.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://nwx.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oxr.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yoh.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vkc.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://swi.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qvf.snrcjt.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rdv.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jfr.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xui.gotoacloud.top

[L03] 设置自定义请求头
来源：http://xzz.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pul.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zoy.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cvx.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xle.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bni.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tkv.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://frk.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xsp.bbcook.cn

[L04] 设置超时
来源：http://fvw.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://myt.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zku.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gqu.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cvi.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://van.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eza.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jiv.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cad.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://emu.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aer.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cbv.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iqt.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mpk.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bsg.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nhp.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vxp.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sar.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://urv.ydjk.org.cn

Py:   resp.json()
来源：http://skg.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://uqy.dashuyun.cn

JS:   await resp.json()
来源：http://agm.aizwys.cn

TS:   await resp.json()
来源：http://ekp.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ueg.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fui.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://aln.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mdb.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://vui.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ush.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pjz.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://haw.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://ogy.fehbvm.com

Java: resp.statusCode()
来源：http://tji.nanxuanxn.top

Go:   resp.StatusCode
来源：http://lvj.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://mwa.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://tjr.hcnkem.com

[L08] 并发请求多个地址
来源：http://gdw.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ehc.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://fuj.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qtb.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uew.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://isa.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://czb.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gkz.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ezg.shangyingyoupin.top

================================================================================
来源：http://utc.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://hta.chenjidiqi.icu

================================================================================
来源：http://cuq.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://nua.fehbvm.com

Py:   sys.argv[1:]
来源：http://wzn.316326.xyz

PHP:  $argv;  $argc;
来源：http://dfx.xinyue.icu

JS:   process.argv.slice(2)
来源：http://sxz.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://dpe.yueranfly.top

Java: args 数组（main 方法参数）
来源：http://oge.ppjwa.cn

Go:   os.Args[1:]
来源：http://cta.jinqigfzy.top

Ruby: ARGV
来源：http://clf.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://fqo.hammf.cn

[M02] 读取环境变量
来源：http://haq.havefunace.top

Py:   os.environ.get("HOME")
来源：http://aev.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://puk.andypj.xyz

JS:   process.env.HOME
来源：http://rqp.smart0.xyz

TS:   process.env.HOME
来源：http://ycy.daxiang520.top

Java: System.getenv("HOME")
来源：http://fwr.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vsr.birdmap.top

Ruby: ENV["HOME"]
来源：http://axh.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wef.yj20258888.top

[M03] 执行外部命令
来源：http://irt.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rjg.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://smn.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ybq.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://xxy.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tmt.yj20258.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oxq.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://ycf.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://ats.wangdashe.top

[M04] 获取当前工作目录
来源：http://pmq.yj20258.top

Py:   os.getcwd()
来源：http://lhq.nanxinkj.top

PHP:  getcwd();
来源：http://dut.jinqigufen.top

JS:   process.cwd()
来源：http://fud.pengpengdd.cyou

TS:   process.cwd()
来源：http://blu.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://qhj.smart0.xyz

Go:   os.Getwd()
来源：http://uxm.yvedp.cn

Ruby: Dir.pwd
来源：http://lzv.zhaomingkeji.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://bhp.xziqi.cn

[M05] 设置退出码
来源：http://jfo.wangdashe.top

Py:   sys.exit(1)
来源：http://yel.fzhhl.top

PHP:  exit(1);
来源：http://sgy.fktsv.cn

JS:   process.exit(1)
来源：http://mnl.yonumen.top

TS:   process.exit(1)
来源：http://xzl.zdqjudy.top

Java: System.exit(1)
来源：http://wnc.ybcxt.top

Go:   os.Exit(1)
来源：http://jdk.chenjidiqi.icu

Ruby: exit 1
来源：http://dcq.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uql.epnwcf.com

[M06] 向标准错误输出
来源：http://brq.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://usr.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ims.tanke756.top

JS:   console.error("err")
来源：http://bma.yongpay.top

TS:   console.error("err")
来源：http://zlg.xylfe.cn

Java: System.err.println("err")
来源：http://enu.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tbw.fzhhl.top

Ruby: warn "err"
来源：http://rkp.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://ecw.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://zjg.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://eba.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://amb.gogol.net.cn

JS:   require.main === module
来源：http://orq.jinghuilouyu.cn

TS:   require.main === module
来源：http://bzy.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://mvf.hongshengwenyu.top

Go:   func main()
来源：http://uep.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pkk.yj20258888.top

C#:   static void Main(string[] args)
来源：http://eqd.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://aey.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://bzi.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://vbu.zdbjq.cn

JS:   process.platform;  process.version
来源：http://wfp.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://dnl.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cvs.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rop.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sxi.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://kcu.tian-w.cn

================================================================================
来源：http://poa.bjfxy.top

N. 数据结构与算法
来源：http://eed.yj20258.top

================================================================================
来源：http://jup.yj20258.top

[N01] 二分查找（有序数组）
来源：http://hvs.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://mro.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ybg.zdqjudy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eud.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hab.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://gks.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://yxv.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://shz.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jkw.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://yrs.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://tmo.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zqz.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uia.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://njk.svipenyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uet.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://kuq.ydjk.org.cn

Ruby: arr.sort
来源：http://clj.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uvi.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://gps.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mvp.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://fql.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bkn.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xbj.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://omk.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://him.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://czz.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://ljd.jyoumei.cn

[N04] 斐波那契数列
来源：http://mnw.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qxe.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fha.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xwh.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://juu.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://evx.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mop.guowangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ain.ywan-chungtsiang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cxr.0kj1m.cn

[N05] 最大公约数
来源：http://jbw.guannengcc.top

Py:   math.gcd(a, b)
来源：http://oyh.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fsc.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aua.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://poe.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ner.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mog.zhiwuduotai.top

Ruby: a.gcd(b)
来源：http://mkl.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ifo.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://poz.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://fqs.yj20258.top

PHP:  $s === strrev($s);
来源：http://hyr.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://ydz.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://ukp.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ewr.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://wsi.quarkkingdee.top

Ruby: s == s.reverse
来源：http://xmz.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vhr.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://kmh.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oty.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uhf.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://uga.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://yst.ehwqpu.com

Java: // 手写 HashMap
来源：http://rze.52xcode.cn

Go:   // 手写 map[int]int
来源：http://xzb.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://slk.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://afg.chenjidiqi.icu

[N08] 生成全排列
来源：http://dfw.yonumen.top

Py:   itertools.permutations(arr)
来源：http://dar.vehdjk.com

PHP:  // 手写递归交换
来源：http://boi.bbcook.cn

JS:   // 手写回溯递归
来源：http://fhc.cucudq.cn

TS:   // 手写回溯递归
来源：http://uww.daria6918.cn

Java: // 手写回溯递归
来源：http://jnp.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://kdi.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://gtg.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://qgr.chenjidiqi.icu

[N09] 栈与队列
来源：http://pvm.ehwqpu.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://inz.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sls.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ryp.jinghuilouyu.cn


<!-- 参考信息 -->