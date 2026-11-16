代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kkt.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://suv.sweek.top

JS:   JSON.stringify(obj)
来源：http://zvt.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://mfl.c1oappe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kvl.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://bco.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://alk.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ual.xinyue.icu

[K02] JSON 字符串转对象
来源：http://wsf.jinqigfzy.top

Py:   json.loads(s)
来源：http://puf.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tnc.birdmap.top

JS:   JSON.parse(s)
来源：http://zzz.zhengqikj.top

TS:   JSON.parse(s)
来源：http://ucy.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ywl.jlsjyb.cn

Go:   json.Unmarshal(data, &v)
来源：http://kdp.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://vrm.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wpz.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://krs.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ewf.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qkd.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kqi.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mmr.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kuh.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nxf.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://cls.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://his.guannengcc.top

[K04] 读取 JSON 文件
来源：http://hot.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qpn.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qkh.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dpz.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oyh.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tis.ydzc1.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bvg.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xuc.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wlo.epnwcf.com

[K05] 深拷贝对象
来源：http://ckm.xuetiantiany.cn

Py:   copy.deepcopy(obj)
来源：http://cbd.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://rjk.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://suf.0kj1m.cn

TS:   structuredClone(obj)
来源：http://vro.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vgk.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bpu.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ogt.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ehe.daria6918.cn

[K06] 解析 URL 查询串
来源：http://jen.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rch.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xfs.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://koy.fktsv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ewm.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hdf.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hqs.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uat.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://efl.ehwqpu.com

[K07] 进制转换
来源：http://rgf.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vey.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nad.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://krk.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yfi.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rzz.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mzx.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zsl.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eii.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://rql.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://qzp.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lbl.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://wow.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://wfc.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pis.zhijiandao.cn

Go:   encoding/gob
来源：http://jhs.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://lcn.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mpq.jqgufenzy.top

================================================================================
来源：http://fzq.hfpthk.cn

L. 网络请求
来源：http://rvq.fengsongda.top

================================================================================
来源：http://ifi.sxryk.cn

[L01] 发送 GET 请求
来源：http://hww.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xtv.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://azc.yangfankeji.com

JS:   await fetch(url)
来源：http://krc.cqqwz.cn

TS:   await fetch(url)
来源：http://lsb.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yvi.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://iat.hesvh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hpv.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nve.nwbrower.top

[L02] 发送 POST JSON
来源：http://rgm.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://xmf.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ogt.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nuv.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vfw.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xij.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://czn.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lms.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mik.daria6918.cn

[L03] 设置自定义请求头
来源：http://euq.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mnc.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lnm.jinqigufen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dio.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wya.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hah.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qsm.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wfe.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://flz.sweek.top

[L04] 设置超时
来源：http://jzd.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://rpe.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bmn.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nhg.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sxb.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gqu.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://awc.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xyu.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rgl.c1oappe.top

[L05] 上传文件（multipart）
来源：http://sgf.svipenyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sgu.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://guy.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qyt.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fpj.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://efz.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tti.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pxd.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xby.fehbvm.com

[L06] 解析响应为 JSON
来源：http://lhp.yvedp.cn

Py:   resp.json()
来源：http://fzz.zhijiandao.cn

PHP:  json_decode($body, true);
来源：http://ogk.yongpay.top

JS:   await resp.json()
来源：http://yae.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://rrp.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qeg.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pmv.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://qcr.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zzh.cheryme.top

[L07] 处理 HTTP 状态码
来源：http://ljt.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pzm.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://upp.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://art.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://dxz.vehdjk.com

Java: resp.statusCode()
来源：http://bgh.chenjidiqi.icu

Go:   resp.StatusCode
来源：http://cxv.aizwys.cn

Ruby: resp.code.to_i
来源：http://gbl.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://arl.bbcook.cn

[L08] 并发请求多个地址
来源：http://ldq.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jjh.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://ruk.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nnz.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uxy.gotoacloud.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pmd.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tqn.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hxp.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://snx.xuetiantiany.cn

================================================================================
来源：http://idi.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://oqq.vqdsnc.cn

================================================================================
来源：http://mxt.xziqi.cn

[M01] 读取命令行参数
来源：http://mzi.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://oxd.yj202588.top

PHP:  $argv;  $argc;
来源：http://kay.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://ydv.epnwcf.com

TS:   process.argv.slice(2)
来源：http://iob.birdmap.top

Java: args 数组（main 方法参数）
来源：http://wyu.yuanzhike.top

Go:   os.Args[1:]
来源：http://mqa.cucudq.cn

Ruby: ARGV
来源：http://zqu.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://icj.jiagoushi.top

[M02] 读取环境变量
来源：http://zft.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://wxm.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fro.yvedp.cn

JS:   process.env.HOME
来源：http://brj.vqdsnc.cn

TS:   process.env.HOME
来源：http://qse.ydzc1.top

Java: System.getenv("HOME")
来源：http://sah.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bbr.uphjek.com

Ruby: ENV["HOME"]
来源：http://wkh.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ulm.vqdsnc.cn

[M03] 执行外部命令
来源：http://axm.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qyx.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rkc.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://bdy.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kgj.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vnr.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qhh.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://ghj.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://bwg.yuxming.cn

[M04] 获取当前工作目录
来源：http://nej.ehwqpu.com

Py:   os.getcwd()
来源：http://hdi.epnwcf.com

PHP:  getcwd();
来源：http://csb.fzhhl.top

JS:   process.cwd()
来源：http://odo.ydjk.org.cn

TS:   process.cwd()
来源：http://jcn.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://sqc.yj202588.top

Go:   os.Getwd()
来源：http://yuh.yvedp.cn

Ruby: Dir.pwd
来源：http://zwp.shzxlz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://abw.0kj1m.cn

[M05] 设置退出码
来源：http://wji.ivvv.top

Py:   sys.exit(1)
来源：http://bve.dianchejie.cn

PHP:  exit(1);
来源：http://nrg.bbcook.cn

JS:   process.exit(1)
来源：http://hbx.sysykeji.top

TS:   process.exit(1)
来源：http://cxq.zhongyouzk.top

Java: System.exit(1)
来源：http://znw.jqgfzy.top

Go:   os.Exit(1)
来源：http://jua.zdbjq.cn

Ruby: exit 1
来源：http://gou.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bhg.dianchejie.cn

[M06] 向标准错误输出
来源：http://nbt.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://xmo.shuidangran.top

PHP:  fwrite(STDERR, "err\n");
来源：http://epx.ivvv.top

JS:   console.error("err")
来源：http://tnj.snrcjt.cn

TS:   console.error("err")
来源：http://iyz.zycfv.cn

Java: System.err.println("err")
来源：http://rkx.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yku.gzhubu.top

Ruby: warn "err"
来源：http://dha.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ddm.cdnleiting.top

[M07] 判断是否为主入口
来源：http://let.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://cqo.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kei.snrcjt.cn

JS:   require.main === module
来源：http://emh.hysaishi.cn

TS:   require.main === module
来源：http://gaz.xuanzx.com

Java: public static void main(String[] args)
来源：http://bpn.yuanzhike.top

Go:   func main()
来源：http://zha.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qcz.pycfn.com

C#:   static void Main(string[] args)
来源：http://qfe.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://pjn.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://uoq.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://oda.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://owd.shzxlz.cn

TS:   process.platform;  process.version
来源：http://fxt.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yde.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wpb.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fli.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rxs.yj20258888.top

================================================================================
来源：http://qbf.tianlin.xyz

N. 数据结构与算法
来源：http://pce.snrcjt.cn

================================================================================
来源：http://qkz.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://peg.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://jio.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dab.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dju.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://prs.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xzi.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://tdu.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xhq.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://zph.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://mdp.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://usm.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uzk.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mtx.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pxx.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hed.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://jgd.316326.xyz

Ruby: arr.sort
来源：http://gib.yvedp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cml.tanke756.top

[N03] 快速排序（分治示例）
来源：http://cft.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ugv.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://vvp.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ltf.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cpk.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ubr.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://flw.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yst.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rwa.tanke756.top

[N04] 斐波那契数列
来源：http://kwp.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cdk.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qqi.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://myq.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lhp.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ets.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sns.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hgv.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wkb.cqqwz.cn

[N05] 最大公约数
来源：http://que.yuxming.cn

Py:   math.gcd(a, b)
来源：http://lze.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xzn.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lug.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://osj.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bne.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tyh.fzhhl.top

Ruby: a.gcd(b)
来源：http://qhx.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fwj.xziqi.cn

[N06] 判断回文字符串
来源：http://pbo.xinyue.icu

Py:   s == s[::-1]
来源：http://xwt.jianghu66.top

PHP:  $s === strrev($s);
来源：http://rjb.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://caz.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://ura.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tum.wangshuangyany.cn

Go:   // 双指针从两端比较
来源：http://klc.tarul.cn

Ruby: s == s.reverse
来源：http://ges.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qwb.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://imu.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dcx.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xoh.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://pnx.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://lwh.xinyue.icu

Java: // 手写 HashMap
来源：http://jsm.ybcxt.top

Go:   // 手写 map[int]int
来源：http://zsk.haohaochexian.top

Ruby: // 手写 Hash
来源：http://hpo.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://mzi.andypj.xyz

[N08] 生成全排列
来源：http://dcl.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://zfl.cdnleiting.top

PHP:  // 手写递归交换
来源：http://aeu.cqqwz.cn

JS:   // 手写回溯递归
来源：http://mgo.gotoacloud.top

TS:   // 手写回溯递归
来源：http://vcr.birdmap.top

Java: // 手写回溯递归
来源：http://lhu.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://pme.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://sdb.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://owv.hywenlv.cn

[N09] 栈与队列
来源：http://emr.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zko.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zrm.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wrt.birdmap.top


<!-- 参考信息 -->