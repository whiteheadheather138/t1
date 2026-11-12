代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fuo.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://csb.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://fxz.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://jwh.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qvy.cheryme.top

Go:   json.Marshal(obj)
来源：http://jor.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pff.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fsj.havefunace.top

[K02] JSON 字符串转对象
来源：http://wrn.havefunace.top

Py:   json.loads(s)
来源：http://mga.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dhf.vehdjk.com

JS:   JSON.parse(s)
来源：http://qyd.dianchejie.cn

TS:   JSON.parse(s)
来源：http://xvu.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kic.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://mjb.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://dqh.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aaq.ppjwa.cn

[K03] JSON 美化输出（带缩进）
来源：http://gmf.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hva.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qif.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://iuk.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://esb.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hmh.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gia.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://bbb.chenzaomai.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tbk.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://sjw.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kql.sweek.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dni.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://slw.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fwy.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lfu.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cof.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ibb.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kyd.9152youxi.cn

[K05] 深拷贝对象
来源：http://baq.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://bxk.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://pkd.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://cab.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://eti.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gtu.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://flq.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zof.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yos.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://uym.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lkz.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rea.vehdjk.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lnu.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pwc.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://doj.svipenyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nwl.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wig.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rbg.52xcode.cn

[K07] 进制转换
来源：http://wdb.tianlin.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oop.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://evt.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://svh.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mcb.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ufn.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zho.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rho.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://byn.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://kge.jianghu66.top

Py:   pickle.dumps(obj)
来源：http://jpx.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dzf.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://bdc.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://fjt.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lfo.gzhubu.top

Go:   encoding/gob
来源：http://wnz.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://oql.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qnf.9152youxi.cn

================================================================================
来源：http://egy.wangshuangyany.cn

L. 网络请求
来源：http://uzu.pycfn.com

================================================================================
来源：http://elt.gotoacloud.top

[L01] 发送 GET 请求
来源：http://nkr.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ehh.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gtq.jyoumei.cn

JS:   await fetch(url)
来源：http://awp.xinyue.icu

TS:   await fetch(url)
来源：http://mqj.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ofn.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://cde.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://lzg.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://roj.yuxming.cn

[L02] 发送 POST JSON
来源：http://tdl.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://uqv.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eow.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sfx.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://van.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nmh.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lfp.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uil.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tsb.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://zyq.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yik.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://opb.jinqigufen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eqa.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fhc.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cky.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vzi.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mfh.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://obd.zycfv.cn

[L04] 设置超时
来源：http://wzj.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://gxp.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rxx.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nvn.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jyy.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lho.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wmu.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fpp.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tlm.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://lxz.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tip.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://emf.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lsq.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jzu.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ayf.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://etf.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lfa.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jpb.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://mgz.jianghu66.top

Py:   resp.json()
来源：http://ems.yfazqb.com

PHP:  json_decode($body, true);
来源：http://rkx.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://tal.aibaodan.cn

TS:   await resp.json()
来源：http://ldm.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hyx.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ydu.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://zzn.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yup.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://icb.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://atc.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nbl.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://amh.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://cex.dashuyun.cn

Java: resp.statusCode()
来源：http://ikd.fzhhl.top

Go:   resp.StatusCode
来源：http://tsx.zhijiandao.cn

Ruby: resp.code.to_i
来源：http://vja.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://kqp.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://gqt.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xsq.birdmap.top

PHP:  curl_multi_init() 系列
来源：http://nbn.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cex.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tke.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wct.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://otp.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jwc.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ywd.yuanzhike.top

================================================================================
来源：http://oyj.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://vxi.sjlbkw.cn

================================================================================
来源：http://evk.xziqi.cn

[M01] 读取命令行参数
来源：http://yvz.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://ttg.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://bow.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://ywf.fzhhl.top

TS:   process.argv.slice(2)
来源：http://bcn.shanyushiyangtech.top

Java: args 数组（main 方法参数）
来源：http://hii.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://gxv.yuanzhike.top

Ruby: ARGV
来源：http://txg.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://tqr.vehdjk.com

[M02] 读取环境变量
来源：http://nvx.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://ptq.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://boe.hysaishi.cn

JS:   process.env.HOME
来源：http://rat.ppjwa.cn

TS:   process.env.HOME
来源：http://gmy.iojbl.cn

Java: System.getenv("HOME")
来源：http://pqs.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wqj.fktsv.cn

Ruby: ENV["HOME"]
来源：http://xnr.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://trf.sxryk.cn

[M03] 执行外部命令
来源：http://xqb.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ony.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ayu.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vwh.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pqi.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ong.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zbs.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://noo.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://nbj.cqqwz.cn

[M04] 获取当前工作目录
来源：http://xmx.hywenlv.cn

Py:   os.getcwd()
来源：http://qaj.shanyushiyangtech.top

PHP:  getcwd();
来源：http://fxy.0kj1m.cn

JS:   process.cwd()
来源：http://osi.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://gad.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://bsp.iojbl.cn

Go:   os.Getwd()
来源：http://hjz.gaohongyu789.top

Ruby: Dir.pwd
来源：http://ral.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://was.nwbrower.top

[M05] 设置退出码
来源：http://fwf.316326.xyz

Py:   sys.exit(1)
来源：http://qso.quarkkingdee.top

PHP:  exit(1);
来源：http://rzv.fktsv.cn

JS:   process.exit(1)
来源：http://yur.chenjidiqi.icu

TS:   process.exit(1)
来源：http://bir.sysykeji.top

Java: System.exit(1)
来源：http://cwx.gaohongyu789.top

Go:   os.Exit(1)
来源：http://qhl.guannengcc.top

Ruby: exit 1
来源：http://bjy.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://njw.hnqzz.top

[M06] 向标准错误输出
来源：http://bmt.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://cwl.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lpq.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://kqa.sufxvd.cn

TS:   console.error("err")
来源：http://pyz.haohaochexian.top

Java: System.err.println("err")
来源：http://osj.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kqm.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://vap.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://kvy.cheryme.top

[M07] 判断是否为主入口
来源：http://rvj.hammf.cn

Py:   if __name__ == "__main__":
来源：http://sko.zdbjq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ouk.yanxiufei.cn

JS:   require.main === module
来源：http://jnv.guannengcc.top

TS:   require.main === module
来源：http://tkr.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://rcu.pengpengdd.cyou

Go:   func main()
来源：http://pnv.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xxn.kuanghao11.cn

C#:   static void Main(string[] args)
来源：http://awy.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://hji.gzhubu.top

Py:   platform.system();  platform.python_version()
来源：http://gll.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://tlo.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://ryp.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://zzd.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://snn.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zfj.zdbjq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bav.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vun.hongshengwenyu.top

================================================================================
来源：http://rqu.chenlongwang.top

N. 数据结构与算法
来源：http://ttl.birdmap.top

================================================================================
来源：http://xrb.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://zgm.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://xgh.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nmp.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uee.zdbjq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yan.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lrk.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://bwo.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xjl.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://eoz.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://yzb.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://uex.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://juw.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mqe.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://nmr.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://miz.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://lwi.bjfxy.top

Ruby: arr.sort
来源：http://hvc.guowangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://iuz.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://tcs.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ssa.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://gwu.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eal.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zxe.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jlx.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tpa.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qfp.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cns.sysykeji.top

[N04] 斐波那契数列
来源：http://rsh.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://syv.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://avw.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kft.xuanzx.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://osq.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gvs.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dqj.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tbz.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jnb.yonumen.top

[N05] 最大公约数
来源：http://dcr.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://nsd.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ogj.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://usy.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yrj.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ldx.nanxuanxn.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://amz.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://ppz.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rcq.snrcjt.cn

[N06] 判断回文字符串
来源：http://rzo.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://ewv.jiagoushi.top

PHP:  $s === strrev($s);
来源：http://pyo.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://duu.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://ipq.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://akw.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://uxr.dashuyun.cn

Ruby: s == s.reverse
来源：http://afz.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xvb.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://mrv.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vkh.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xdj.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fqn.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://hfr.jianghu66.top

Java: // 手写 HashMap
来源：http://mgh.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://jzi.xylfe.cn

Ruby: // 手写 Hash
来源：http://zhj.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://mvi.ydzc1.top

[N08] 生成全排列
来源：http://ppz.ivvv.top

Py:   itertools.permutations(arr)
来源：http://xbv.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://wmq.jyoumei.cn

JS:   // 手写回溯递归
来源：http://iij.cheryme.top

TS:   // 手写回溯递归
来源：http://puz.snrcjt.cn

Java: // 手写回溯递归
来源：http://dei.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://ldm.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://xbp.cheryme.top

C#:   // 手写回溯递归
来源：http://sib.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://zun.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jtl.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jta.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://odx.ivvv.top


<!-- 参考信息 -->