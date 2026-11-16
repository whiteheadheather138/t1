代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rgn.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cqn.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://lsj.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://bwy.sxryk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wqq.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://fha.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ink.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uny.wangdashe.top

[K02] JSON 字符串转对象
来源：http://lir.zhiwuduotai.top

Py:   json.loads(s)
来源：http://mqv.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tyq.nanxinkj.top

JS:   JSON.parse(s)
来源：http://dww.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://wtk.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yxc.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://irw.andypj.xyz

Ruby: JSON.parse(s)
来源：http://ebw.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://upb.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://tya.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ctl.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://whj.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xez.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nax.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://avy.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oxt.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dyo.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zwa.yonumen.top

[K04] 读取 JSON 文件
来源：http://dly.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jii.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://plg.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dxd.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://irv.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://usz.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nmo.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bht.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zrv.pycfn.com

[K05] 深拷贝对象
来源：http://aao.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://uzq.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://qvr.tian-w.cn

JS:   structuredClone(obj)
来源：http://bap.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://zcb.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://htk.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ucn.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qte.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lcv.shuidangran.top

[K06] 解析 URL 查询串
来源：http://mbh.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vcw.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vaq.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rdr.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hfu.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nlc.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gpc.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ndh.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pzi.gaohongyu789.top

[K07] 进制转换
来源：http://sxo.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://htr.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vyl.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eev.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vwb.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xrl.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vyk.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cer.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wat.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://yzw.shangyingyoupin.top

Py:   pickle.dumps(obj)
来源：http://cbb.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ryb.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://eoy.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://cem.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ulc.yj202588.top

Go:   encoding/gob
来源：http://fan.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://bod.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yho.sweek.top

================================================================================
来源：http://twq.9152youxi.cn

L. 网络请求
来源：http://sdc.tianlin.xyz

================================================================================
来源：http://xrr.uphjek.com

[L01] 发送 GET 请求
来源：http://lpn.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uvb.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xdf.sweek.top

JS:   await fetch(url)
来源：http://scy.andypj.xyz

TS:   await fetch(url)
来源：http://tcf.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jbn.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://xqu.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tuo.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wvc.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://miz.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://zgl.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uyh.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ule.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nod.meibo888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ikj.snrcjt.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bll.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rub.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ucj.52xcode.cn

[L03] 设置自定义请求头
来源：http://wck.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fdh.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oje.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqv.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zey.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://snk.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oum.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xjr.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dmn.wangdashe.top

[L04] 设置超时
来源：http://wsb.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://qxu.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jfy.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ugd.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ezx.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qeg.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ivj.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xlz.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://klz.cashguo.top

[L05] 上传文件（multipart）
来源：http://hww.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jka.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dcb.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zet.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xvn.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sxf.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jsn.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://knx.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gko.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://mvg.tanke756.top

Py:   resp.json()
来源：http://dhq.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://izm.guannengcc.top

JS:   await resp.json()
来源：http://xuk.aibaodan.cn

TS:   await resp.json()
来源：http://puu.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://psp.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://amk.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://vnf.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dkp.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://hgx.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jef.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ghs.yj202588.top

JS:   resp.ok;  resp.status
来源：http://gzp.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://hyc.shangyingyoupin.top

Java: resp.statusCode()
来源：http://szm.pycfn.com

Go:   resp.StatusCode
来源：http://qgc.daria6918.cn

Ruby: resp.code.to_i
来源：http://aqk.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://jyr.zdqjudy.top

[L08] 并发请求多个地址
来源：http://fkd.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://evv.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://ndn.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://swq.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://axh.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dye.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mwr.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wvf.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eek.kuanghao11.cn

================================================================================
来源：http://grk.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://foo.ppjwa.cn

================================================================================
来源：http://ahr.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://bso.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://wqk.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://pbo.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://xfu.sweek.top

TS:   process.argv.slice(2)
来源：http://nfz.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://vxy.sweek.top

Go:   os.Args[1:]
来源：http://wrg.cqqwz.cn

Ruby: ARGV
来源：http://hmz.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://ezp.pengpengdd.cyou

[M02] 读取环境变量
来源：http://ouy.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://mao.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vrx.sweek.top

JS:   process.env.HOME
来源：http://rxb.0kj1m.cn

TS:   process.env.HOME
来源：http://ycl.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://tng.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jqh.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://gzr.yuxming.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qxn.ehwqpu.com

[M03] 执行外部命令
来源：http://jzz.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kym.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mdg.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oce.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ayp.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ymx.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://gie.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://knd.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://fzk.sxryk.cn

[M04] 获取当前工作目录
来源：http://wiy.quarkkingdee.top

Py:   os.getcwd()
来源：http://zlt.aibaodan.cn

PHP:  getcwd();
来源：http://aap.mhx1999.top

JS:   process.cwd()
来源：http://eid.chenlongwang.top

TS:   process.cwd()
来源：http://cns.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://kmg.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://fud.quarkkingdee.top

Ruby: Dir.pwd
来源：http://ogs.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://smp.bjfxy.top

[M05] 设置退出码
来源：http://ksj.0kj1m.cn

Py:   sys.exit(1)
来源：http://khy.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://pyf.mhx1999.top

JS:   process.exit(1)
来源：http://lpo.chenlongwang.top

TS:   process.exit(1)
来源：http://akr.yj202588.top

Java: System.exit(1)
来源：http://eja.hesvh.cn

Go:   os.Exit(1)
来源：http://hlp.gaohongyu789.top

Ruby: exit 1
来源：http://ihv.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oaq.chenlongwang.top

[M06] 向标准错误输出
来源：http://ntq.hfpthk.cn

Py:   print("err", file=sys.stderr)
来源：http://luz.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://tnf.yonumen.top

JS:   console.error("err")
来源：http://evd.shanyushiyangtech.top

TS:   console.error("err")
来源：http://snz.xuanzx.com

Java: System.err.println("err")
来源：http://mjb.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://itn.yangfankeji.com

Ruby: warn "err"
来源：http://lzz.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://rur.jiagoushi.top

[M07] 判断是否为主入口
来源：http://hnk.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://dqj.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vat.0kj1m.cn

JS:   require.main === module
来源：http://wwx.wangdashe.top

TS:   require.main === module
来源：http://rhk.zhengqikj.top

Java: public static void main(String[] args)
来源：http://oqv.chenzaomai.com

Go:   func main()
来源：http://nfl.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ome.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://mfq.hammf.cn

[M08] 获取系统与运行时信息
来源：http://lke.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://yoj.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://aru.ybcxt.top

JS:   process.platform;  process.version
来源：http://tnq.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://rkq.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xad.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ivx.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zkv.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://qqu.aibaodan.cn

================================================================================
来源：http://nyh.gaohongyu789.top

N. 数据结构与算法
来源：http://dqn.nanxuanxn.top

================================================================================
来源：http://wzi.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://fgc.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://cpq.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gdv.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ono.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ncd.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://kbn.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://hbp.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jgk.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://drn.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://qvh.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://jpy.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mya.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kfl.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://syc.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xkc.mhx1999.top

Go:   slices.Sort(arr)
来源：http://oez.andypj.xyz

Ruby: arr.sort
来源：http://upl.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://hty.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://yoc.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fho.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://kqy.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fwu.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lbq.fzhhl.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vnz.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sml.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tky.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://bmw.jqgufenzy.top

[N04] 斐波那契数列
来源：http://zwz.ybcxt.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jdu.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qnf.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hoi.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hqz.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eiw.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lca.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sqf.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tfc.epnwcf.com

[N05] 最大公约数
来源：http://siy.yonumen.top

Py:   math.gcd(a, b)
来源：http://akt.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cfh.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nwo.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://huo.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rkp.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zwb.haohaochexian.top

Ruby: a.gcd(b)
来源：http://ozd.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vnm.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://qcd.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://gck.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://xzg.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://gcd.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://qoq.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://txa.yj20258888.top

Go:   // 双指针从两端比较
来源：http://cvv.jianghu66.top

Ruby: s == s.reverse
来源：http://nej.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ipp.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://edq.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ubx.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hku.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://goy.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://aza.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://xxg.jianghu66.top

Go:   // 手写 map[int]int
来源：http://nfo.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://ixy.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://gcf.hywenlv.cn

[N08] 生成全排列
来源：http://juj.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://bym.yj202588.top

PHP:  // 手写递归交换
来源：http://hil.wangshuangyany.cn

JS:   // 手写回溯递归
来源：http://tfr.tianlin.xyz

TS:   // 手写回溯递归
来源：http://bed.yuxming.cn

Java: // 手写回溯递归
来源：http://gwt.uphjek.com

Go:   // 手写回溯递归
来源：http://qjf.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://nlc.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://zlg.316326.xyz

[N09] 栈与队列
来源：http://usc.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hjz.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fhh.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ewe.ydzc1.top


<!-- 参考信息 -->