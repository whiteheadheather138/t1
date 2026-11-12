代发 wailian999

Ruby: attr_accessor :name
来源：http://cko.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://nbd.hcnkem.com

[G12] 对象转字符串
来源：http://cqh.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://wis.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wnn.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://jwm.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://pkx.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://tqk.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://snp.vqdsnc.cn

Ruby: def to_s; @name; end
来源：http://oqu.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://sou.haohaochexian.top

[G13] 判断对象类型
来源：http://igf.fehbvm.com

Py:   isinstance(u, User)
来源：http://uxs.guannengcc.top

PHP:  $u instanceof User
来源：http://lef.pycfn.com

JS:   u instanceof User
来源：http://dzl.bjfxy.top

TS:   u instanceof User
来源：http://cbe.yongpay.top

Java: u instanceof User
来源：http://gno.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vdc.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://bgf.havefunace.top

C#:   u is User
来源：http://zor.epnwcf.com

[G14] 数据类 / record
来源：http://lrl.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gfu.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://lpr.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://auu.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://xyb.guannengcc.top

Java: record User(String name, int age) {}
来源：http://ciz.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://xwx.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xyb.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://jod.havefunace.top

[G15] 枚举
来源：http://xnp.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jry.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hdy.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://itp.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wsv.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://pbr.tianlin.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qnh.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://oyh.cashguo.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wan.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://ubx.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dag.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://rrr.sysykeji.top

JS:   Object.entries(obj)
来源：http://bde.bbcook.cn

TS:   Object.entries(obj)
来源：http://zim.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vhe.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kkb.dashuyun.cn

Ruby: obj.instance_variables
来源：http://lvg.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://riw.gzhubu.top

================================================================================
来源：http://nnp.0kj1m.cn

H. 异常与错误处理
来源：http://dwb.zhaomingkeji.xyz

================================================================================
来源：http://ubo.mhx1999.top

[H01] try / catch 基础
来源：http://veo.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hzv.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://syy.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qaw.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hcm.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rco.jinqigfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tay.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xgw.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yta.yuxming.cn

[H02] finally / ensure 收尾
来源：http://gaq.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://fpb.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://zuc.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://czd.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://qru.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://aqx.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yxt.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kjg.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fxb.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://rev.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://qoa.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://frq.yonumen.top

JS:   throw new Error("错误信息");
来源：http://gxz.hcnkem.com

TS:   throw new Error("错误信息");
来源：http://fjn.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://szc.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tcv.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jtv.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://chl.hesvh.cn

[H04] 自定义异常类型
来源：http://wzi.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://nmj.redwolf501.top

PHP:  class MyError extends RuntimeException {}
来源：http://uoc.yj20258888.top

JS:   class MyError extends Error {}
来源：http://muy.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://xzh.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://how.zdbjq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pjm.chenzaomai.com

Ruby: class MyError < StandardError; end
来源：http://ybm.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://qlx.bjfxy.top

[H05] 捕获特定类型
来源：http://adt.yangfankeji.com

Py:   except ValueError as e:
来源：http://ble.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hhh.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://pfp.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://viu.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://wnf.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hes.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://wgs.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gwn.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://iem.fzhhl.top

Py:   value = d.get("k") or default
来源：http://qlr.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://bxe.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zme.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iws.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xxm.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rvv.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://bvm.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://qnu.cdnleiting.top

[H07] 断言
来源：http://inj.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://wjl.hammf.cn

PHP:  assert($x > 0);
来源：http://nwn.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://fff.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://yay.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://tel.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vau.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://wjg.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://kva.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://vuh.havefunace.top

Py:   str(e);  traceback.format_exc()
来源：http://quw.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zsh.birdmap.top

JS:   e.message;  e.stack
来源：http://cbz.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tdc.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://nmy.ydzc1.top

Go:   err.Error()
来源：http://jop.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://hls.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://pdq.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://kuk.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gtk.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hwg.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://svz.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qyz.ywan-chungtsiang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xlm.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xoa.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://qhi.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uoh.c1oappe.top

[H10] 资源自动释放
来源：http://ojl.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://tnz.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bkz.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yjf.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yvj.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xdr.quarkkingdee.top

Go:   defer f.Close()
来源：http://pii.zhijiandao.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nsh.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iyp.aizwys.cn

================================================================================
来源：http://xkw.gaohongyu789.top

I. 正则表达式
来源：http://cjk.zhijiandao.cn

================================================================================
来源：http://sqd.birdmap.top

[I01] 判断是否匹配
来源：http://cyv.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xbi.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://krt.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://ppx.fehbvm.com

TS:   /\d+/.test(s)
来源：http://xkw.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mdy.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://guz.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://lbm.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cwx.andypj.xyz

[I02] 提取所有匹配
来源：http://lcv.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://got.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mzo.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://efr.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://ohp.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sjt.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ydq.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://zhy.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yux.sxryk.cn

[I03] 提取捕获分组
来源：http://gim.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pka.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qfn.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pll.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lsv.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eie.0kj1m.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hfb.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://goy.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wgr.yangfankeji.com

[I04] 正则替换
来源：http://cdp.fzhhl.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nrg.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jvx.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://ldg.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://raq.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://ojf.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zcs.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://czf.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://exc.nanxinkj.top

[I05] 按正则拆分
来源：http://aim.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lsr.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fqs.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://yvq.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://dhn.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://jwk.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jvh.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pzm.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qrx.jinghuilouyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jmf.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gur.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://klk.ehwqpu.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://phb.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gim.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nis.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fmu.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jho.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://muq.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://yct.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sij.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pkx.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xya.chenlongwang.top

TS:   /error/gim
来源：http://lbb.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dfn.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yeb.tanke756.top

Ruby: s.scan(/error/i)
来源：http://tum.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mgk.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://mgm.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://evy.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xlw.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qin.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xnw.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wad.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pts.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://weg.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kuv.bjfxy.top

================================================================================
来源：http://tom.zhengqikj.top

J. 日期与时间
来源：http://lsh.zhengqikj.top

================================================================================
来源：http://cyg.dianchejie.cn

[J01] 获取当前时间
来源：http://klh.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://urz.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aeq.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://wlw.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://hen.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://krh.gzhubu.top

Go:   time.Now()
来源：http://okm.52xcode.cn

Ruby: Time.now
来源：http://qux.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rys.zycfv.cn

[J02] 格式化输出
来源：http://gaj.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://shs.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://luy.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xuq.smart0.xyz

TS:   d.toISOString()
来源：http://qdb.hammf.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mgf.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xdm.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mbo.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ftr.jqgfzy.top

[J03] 字符串解析为日期
来源：http://plk.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wmf.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://crd.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://yay.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://wty.xuanzx.com

Java: LocalDate.parse("2024-01-02")
来源：http://ale.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xur.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://glw.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xzz.tarul.cn

[J04] 时间戳与日期互转
来源：http://hhd.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iow.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://usz.zhoulong.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kyj.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hbm.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lgt.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ilr.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://isw.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dct.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://hdi.meibo888.top

Py:   now + timedelta(days=7)
来源：http://gcj.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pjr.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://elu.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lmi.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://oni.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ono.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://oyu.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://aoa.zhijiandao.cn

[J06] 计算两时间之差
来源：http://gkn.ctjpmb.com

Py:   (end - start).total_seconds()
来源：http://fmk.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://pys.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qzh.guannengcc.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jic.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bbv.vqdsnc.cn

Go:   end.Sub(start).Hours()
来源：http://evv.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://yio.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://roe.ydzc1.top

[J07] 比较两个日期
来源：http://zcz.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://rgf.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ley.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://dws.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://xff.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kgc.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nhf.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://aha.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://wzo.fzhhl.top

[J08] 提取年月日与星期
来源：http://wvi.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mkt.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://olz.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uui.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tas.meibo888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pgi.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jsh.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iau.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mbu.yj20258888.top

[J09] 时区处理
来源：http://zjm.xingfuxueyuan.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qhi.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fpr.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zae.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oxf.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cey.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dhz.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bfy.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nhi.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://wol.xylfe.cn


<!-- 参考信息 -->