代发 wailian999

================================================================================
来源：http://lzf.zdbjq.cn

K. JSON 与序列化
来源：http://ysu.xingfuxueyuan.xyz

================================================================================
来源：http://taq.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://tlk.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bnu.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tpx.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://xjz.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://gpx.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ymg.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://jaa.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://zmp.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bsm.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://ikh.svipenyu.cn

Py:   json.loads(s)
来源：http://wwa.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://isu.meibo888.top

JS:   JSON.parse(s)
来源：http://dqz.daria6918.cn

TS:   JSON.parse(s)
来源：http://fan.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wby.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://njb.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://qaj.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vpe.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://lqz.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pgm.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qzn.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uun.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sqh.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qkp.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ing.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://pgj.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jhe.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://oux.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pff.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pav.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ofx.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pte.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ymz.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iup.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://gdx.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sen.jinqigfzy.top

[K05] 深拷贝对象
来源：http://jel.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://ngz.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://gmc.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://fms.xuanzx.com

TS:   structuredClone(obj)
来源：http://rop.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yfn.nwbrower.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jtc.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vbe.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fod.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://xhz.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://npa.shuidangran.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hii.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uvf.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gqf.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://efu.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://hse.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oxg.xuanzx.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pcr.0kj1m.cn

[K07] 进制转换
来源：http://ule.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ntm.shuidangran.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://elj.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://agm.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hpf.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jqa.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://obm.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zwq.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ksh.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://lvo.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://pet.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kza.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://lxg.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://kmh.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nzn.c1oappe.top

Go:   encoding/gob
来源：http://ckc.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://vff.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aaq.zdbjq.cn

================================================================================
来源：http://mel.sweek.top

L. 网络请求
来源：http://wrd.hammf.cn

================================================================================
来源：http://rjl.iojbl.cn

[L01] 发送 GET 请求
来源：http://tmv.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://egl.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://och.zdbjq.cn

JS:   await fetch(url)
来源：http://jxs.fengsongda.top

TS:   await fetch(url)
来源：http://dqo.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ppt.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://put.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ftq.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fah.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://eyj.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tzn.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jxh.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kkv.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wbj.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rwh.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hyr.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ngr.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://brx.hcnkem.com

[L03] 设置自定义请求头
来源：http://fwr.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rgs.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fxv.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pwe.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wyv.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ljo.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://btv.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ium.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jyq.yongpay.top

[L04] 设置超时
来源：http://pkm.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://adj.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eck.cqqwz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hvw.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wzn.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wig.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://igg.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zub.birdmap.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jlk.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://civ.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cvn.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xzl.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gzz.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wca.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nlr.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lev.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lht.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vqv.iojbl.cn

[L06] 解析响应为 JSON
来源：http://kfe.guowangkeji.top

Py:   resp.json()
来源：http://ofw.fktsv.cn

PHP:  json_decode($body, true);
来源：http://duu.zhongyouzk.top

JS:   await resp.json()
来源：http://zze.shuidangran.top

TS:   await resp.json()
来源：http://gju.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://btb.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dnp.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://mif.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yob.ppjwa.cn

[L07] 处理 HTTP 状态码
来源：http://fwr.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hzs.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vbr.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://slj.yj202588.top

TS:   resp.ok;  resp.status
来源：http://raa.yvedp.cn

Java: resp.statusCode()
来源：http://cgw.cashguo.top

Go:   resp.StatusCode
来源：http://hzc.havefunace.top

Ruby: resp.code.to_i
来源：http://tty.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://pag.meibo888.top

[L08] 并发请求多个地址
来源：http://ekg.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gmv.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://vuy.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rus.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kot.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pza.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gni.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vdt.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bzb.ivvv.top

================================================================================
来源：http://ckn.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://tew.chenzaomai.com

================================================================================
来源：http://voh.gzhubu.top

[M01] 读取命令行参数
来源：http://tpe.9152youxi.cn

Py:   sys.argv[1:]
来源：http://flk.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://bca.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://swj.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://wma.sxryk.cn

Java: args 数组（main 方法参数）
来源：http://xbb.hcnkem.com

Go:   os.Args[1:]
来源：http://top.andypj.xyz

Ruby: ARGV
来源：http://rkd.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://rts.yj202588.top

[M02] 读取环境变量
来源：http://gfr.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://hgt.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bpu.316326.xyz

JS:   process.env.HOME
来源：http://ioj.bbcook.cn

TS:   process.env.HOME
来源：http://hka.fengsongda.top

Java: System.getenv("HOME")
来源：http://sfd.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yau.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://bvd.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kkt.wangdashe.top

[M03] 执行外部命令
来源：http://gal.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ase.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tan.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hls.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dge.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://agx.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://grs.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://rvk.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://pfy.9152youxi.cn

[M04] 获取当前工作目录
来源：http://wgs.cucudq.cn

Py:   os.getcwd()
来源：http://uhm.hongshengwenyu.top

PHP:  getcwd();
来源：http://ijd.fanxiaobao.xyz

JS:   process.cwd()
来源：http://opf.zycfv.cn

TS:   process.cwd()
来源：http://fpn.cashguo.top

Java: Path.of("").toAbsolutePath()
来源：http://yvk.tianlin.xyz

Go:   os.Getwd()
来源：http://lap.xinyue.icu

Ruby: Dir.pwd
来源：http://vfj.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://owz.hammf.cn

[M05] 设置退出码
来源：http://rpc.wangdashe.top

Py:   sys.exit(1)
来源：http://bar.ybcxt.top

PHP:  exit(1);
来源：http://ght.yangfankeji.com

JS:   process.exit(1)
来源：http://isf.yvedp.cn

TS:   process.exit(1)
来源：http://csk.yangfankeji.com

Java: System.exit(1)
来源：http://spo.cheryme.top

Go:   os.Exit(1)
来源：http://kom.uphjek.com

Ruby: exit 1
来源：http://ije.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oaa.zhongyouzk.top

[M06] 向标准错误输出
来源：http://lha.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://hvf.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xnj.fengsongda.top

JS:   console.error("err")
来源：http://ueg.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://imr.yanxiufei.cn

Java: System.err.println("err")
来源：http://tsy.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vec.tianlin.xyz

Ruby: warn "err"
来源：http://zlg.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://gjw.bbcook.cn

[M07] 判断是否为主入口
来源：http://hxf.cheryme.top

Py:   if __name__ == "__main__":
来源：http://qsr.pycfn.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mrj.yj20258.top

JS:   require.main === module
来源：http://mkc.jyoumei.cn

TS:   require.main === module
来源：http://qhy.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://cwh.cdnleiting.top

Go:   func main()
来源：http://qwy.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ono.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://uth.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://czu.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://pxp.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://aiw.jyoumei.cn

JS:   process.platform;  process.version
来源：http://vbq.daxiang520.top

TS:   process.platform;  process.version
来源：http://eeo.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gss.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://svk.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ltb.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zkf.svipenyu.cn

================================================================================
来源：http://hpu.jinqigfzy.top

N. 数据结构与算法
来源：http://zhw.hcnkem.com

================================================================================
来源：http://paj.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://jdo.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://zfh.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fwt.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mmy.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ofh.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://uic.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://vmf.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://diy.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://bro.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://ruu.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://kbx.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zwj.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vjl.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kup.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jdz.uphjek.com

Go:   slices.Sort(arr)
来源：http://eut.zhixingplan.top

Ruby: arr.sort
来源：http://uql.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://eyj.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://vmm.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bxu.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://iox.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tor.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kog.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yqo.shuidangran.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dmd.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zap.zhengqikj.top

C#:   // 手写递归，或 Array.Sort
来源：http://bsb.vehdjk.com

[N04] 斐波那契数列
来源：http://urh.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://efw.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://faq.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gsd.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zfv.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rbq.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://efr.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sei.epnwcf.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bfa.fengsongda.top

[N05] 最大公约数
来源：http://nil.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://loj.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://otp.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://usl.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hxb.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tjt.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jvn.zhixingplan.top

Ruby: a.gcd(b)
来源：http://blh.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vke.aizwys.cn

[N06] 判断回文字符串
来源：http://dvx.yfazqb.com

Py:   s == s[::-1]
来源：http://jdg.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://myi.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://qfq.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://uup.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oza.jiagoushi.top

Go:   // 双指针从两端比较
来源：http://nyt.cqqwz.cn

Ruby: s == s.reverse
来源：http://zap.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zcd.tian-w.cn

[N07] 两数之和（返回下标）
来源：http://ska.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://swv.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pop.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://and.hammf.cn

TS:   // 手写 Map<string, number>
来源：http://qkg.hywenlv.cn

Java: // 手写 HashMap
来源：http://cmd.zhaomingkeji.xyz

Go:   // 手写 map[int]int
来源：http://bgp.xuanzx.com

Ruby: // 手写 Hash
来源：http://znl.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://bna.vehdjk.com

[N08] 生成全排列
来源：http://cvc.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://dug.havefunace.top

PHP:  // 手写递归交换
来源：http://xup.yfazqb.com

JS:   // 手写回溯递归
来源：http://hsd.ehwqpu.com

TS:   // 手写回溯递归
来源：http://ugt.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://tgr.nanxinkj.top

Go:   // 手写回溯递归
来源：http://zjp.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://ksb.jqgfzy.top

C#:   // 手写回溯递归
来源：http://wds.gaohongyu789.top


<!-- 参考信息 -->