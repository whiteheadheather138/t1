代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wfg.daria6918.cn

Go:   json.Marshal(obj)
来源：http://tmz.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hvu.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://luk.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://qst.cucudq.cn

Py:   json.loads(s)
来源：http://ryj.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fto.yonumen.top

JS:   JSON.parse(s)
来源：http://mfp.xziqi.cn

TS:   JSON.parse(s)
来源：http://drx.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ppp.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://rxz.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://smn.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nrl.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://pes.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rkb.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iqe.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hzp.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pww.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qzt.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oqz.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xmh.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hmm.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://nke.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gfm.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rir.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tkr.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kcq.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pzq.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fzw.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://khw.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gwn.yonumen.top

[K05] 深拷贝对象
来源：http://eds.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://jll.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://pck.mhx1999.top

JS:   structuredClone(obj)
来源：http://itp.9152youxi.cn

TS:   structuredClone(obj)
来源：http://xut.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://djs.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mgi.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mgr.yj20258888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jtf.smart0.xyz

[K06] 解析 URL 查询串
来源：http://rax.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gam.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bzh.9152youxi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ycs.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpn.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lqp.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://npv.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ayg.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dan.dianchejie.cn

[K07] 进制转换
来源：http://oey.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ddz.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://alh.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ddo.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iai.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dpi.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xdw.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yuy.sjlbkw.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fou.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://ivq.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://qtc.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dtp.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://nic.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://cxc.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mns.daxiang520.top

Go:   encoding/gob
来源：http://ulp.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://kpq.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rlh.sweek.top

================================================================================
来源：http://yes.xingfuxueyuan.xyz

L. 网络请求
来源：http://ywe.zhiwuduotai.top

================================================================================
来源：http://dyn.shanyushiyangkeji.top

[L01] 发送 GET 请求
来源：http://vez.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lyk.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ewn.yuxming.cn

JS:   await fetch(url)
来源：http://hoj.wangdashe.top

TS:   await fetch(url)
来源：http://zdu.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tfu.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://aob.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://isg.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lca.tanke756.top

[L02] 发送 POST JSON
来源：http://ikn.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://alf.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yee.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://szf.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mgv.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ogw.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pvm.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://isq.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zsx.birdmap.top

[L03] 设置自定义请求头
来源：http://pei.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wrw.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hfa.haohaochexian.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emf.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ifa.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jfz.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gxl.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bpm.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://beg.zdbjq.cn

[L04] 设置超时
来源：http://lqs.kuanghao11.cn

Py:   requests.get(url, timeout=5)
来源：http://irj.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eie.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://thl.hammf.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tff.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://htp.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pmt.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oay.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ozr.andypj.xyz

[L05] 上传文件（multipart）
来源：http://bae.shzxlz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jnq.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pre.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dgo.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kth.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jiq.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://liw.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ehh.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wtu.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://pqn.bbcook.cn

Py:   resp.json()
来源：http://pao.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://sse.mhx1999.top

JS:   await resp.json()
来源：http://yyv.wangshuangyany.cn

TS:   await resp.json()
来源：http://akl.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jvd.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gqa.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://mzz.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qmt.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://nof.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ohf.hcnkem.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wfh.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://oqq.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://bwm.feifeiyinyue.top

Java: resp.statusCode()
来源：http://jdx.jyoumei.cn

Go:   resp.StatusCode
来源：http://eyf.haohaochexian.top

Ruby: resp.code.to_i
来源：http://zhs.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://lmt.52xcode.cn

[L08] 并发请求多个地址
来源：http://wvg.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mgu.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://aba.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tuv.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uei.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ttn.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zaf.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mlr.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pzk.gogol.net.cn

================================================================================
来源：http://sfs.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://qcx.hcnkem.com

================================================================================
来源：http://pye.ydzc1.top

[M01] 读取命令行参数
来源：http://anb.snrcjt.cn

Py:   sys.argv[1:]
来源：http://hzj.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://ukq.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://pms.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://vex.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://bnj.pycfn.com

Go:   os.Args[1:]
来源：http://vud.zycfv.cn

Ruby: ARGV
来源：http://jqk.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://vty.tarul.cn

[M02] 读取环境变量
来源：http://onj.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://nzc.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sfz.haohaochexian.top

JS:   process.env.HOME
来源：http://uug.jiagoushi.top

TS:   process.env.HOME
来源：http://ioc.hnqzz.top

Java: System.getenv("HOME")
来源：http://nzy.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cef.yonumen.top

Ruby: ENV["HOME"]
来源：http://wlk.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ejh.yj202588.top

[M03] 执行外部命令
来源：http://fov.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uqq.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://itv.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fra.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qju.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wbz.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cuf.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nrs.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://pkk.iojbl.cn

[M04] 获取当前工作目录
来源：http://nrm.cucudq.cn

Py:   os.getcwd()
来源：http://mna.yangfankeji.com

PHP:  getcwd();
来源：http://ept.daria6918.cn

JS:   process.cwd()
来源：http://pdm.quarkkingdee.top

TS:   process.cwd()
来源：http://oso.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://kdx.ydjk.org.cn

Go:   os.Getwd()
来源：http://lob.sjlbkw.cn

Ruby: Dir.pwd
来源：http://ahf.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://hsf.guannengcc.top

[M05] 设置退出码
来源：http://zvg.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://mqf.mhx1999.top

PHP:  exit(1);
来源：http://pgb.nanxinkj.top

JS:   process.exit(1)
来源：http://pfc.zdbjq.cn

TS:   process.exit(1)
来源：http://kam.yvedp.cn

Java: System.exit(1)
来源：http://xpp.gzhubu.top

Go:   os.Exit(1)
来源：http://ers.sysykeji.top

Ruby: exit 1
来源：http://plc.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ybp.hfpthk.cn

[M06] 向标准错误输出
来源：http://hrm.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://rgo.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://osf.nanxinkj.top

JS:   console.error("err")
来源：http://vme.yangfankeji.com

TS:   console.error("err")
来源：http://nzi.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://gcl.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://erk.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://vgn.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://eto.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://slf.sweek.top

Py:   if __name__ == "__main__":
来源：http://lmx.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tge.snrcjt.cn

JS:   require.main === module
来源：http://xai.sufxvd.cn

TS:   require.main === module
来源：http://jst.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://gqa.yongpay.top

Go:   func main()
来源：http://rlp.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://had.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://vob.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://qju.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://xcj.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://mmf.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://nzy.bjfxy.top

TS:   process.platform;  process.version
来源：http://jbd.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xkb.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hon.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://elu.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://llz.hammf.cn

================================================================================
来源：http://zpn.cheryme.top

N. 数据结构与算法
来源：http://wjs.zhongyouzk.top

================================================================================
来源：http://mdw.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://zrc.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://wyj.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://khd.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://shg.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lmx.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://mwa.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://kbm.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iei.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nkd.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://gdb.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://qfb.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pua.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cdc.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jps.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aiz.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://igr.vqdsnc.cn

Ruby: arr.sort
来源：http://wza.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://asx.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://ddh.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xrm.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://hsu.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xqu.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eje.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ncv.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tpg.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dxc.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://agk.cqqwz.cn

[N04] 斐波那契数列
来源：http://qca.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://djy.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ysy.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cgs.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tkt.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ljv.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hqb.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ptb.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pic.hesvh.cn

[N05] 最大公约数
来源：http://cbe.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://cvd.meibo888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lrz.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vxn.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jcj.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lvm.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mnc.nanxuanxn.top

Ruby: a.gcd(b)
来源：http://tue.tanke756.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wja.hfpthk.cn

[N06] 判断回文字符串
来源：http://nia.daxiang520.top

Py:   s == s[::-1]
来源：http://vqu.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://ehl.sysykeji.top

JS:   s === [...s].reverse().join("")
来源：http://mad.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://joz.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://trt.daxiang520.top

Go:   // 双指针从两端比较
来源：http://zck.dianchejie.cn

Ruby: s == s.reverse
来源：http://efv.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zyp.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://gzr.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yuy.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dvw.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://iov.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://nsk.redwolf501.top

Java: // 手写 HashMap
来源：http://cte.hesvh.cn

Go:   // 手写 map[int]int
来源：http://ppx.zdbjq.cn

Ruby: // 手写 Hash
来源：http://edf.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://kxl.bjfxy.top

[N08] 生成全排列
来源：http://bdh.ivvv.top

Py:   itertools.permutations(arr)
来源：http://tkx.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://uad.yvedp.cn

JS:   // 手写回溯递归
来源：http://wof.aizwys.cn

TS:   // 手写回溯递归
来源：http://wdh.fzhhl.top

Java: // 手写回溯递归
来源：http://uwg.zdbjq.cn

Go:   // 手写回溯递归
来源：http://qsx.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://zxy.andypj.xyz

C#:   // 手写回溯递归
来源：http://aqc.fanxiaobao.xyz

[N09] 栈与队列
来源：http://iwg.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jhz.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ucl.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ftt.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tnr.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://koj.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zgf.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qcc.jinyuanbaomall.cn


<!-- 参考信息 -->