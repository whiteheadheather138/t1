代发 wailian999

Ruby: attr_accessor :name
来源：http://ixl.daxiang520.top

C#:   public string Name { get; set; }
来源：http://ohv.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://sea.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://xeq.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qyy.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://ipw.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://qeb.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://axy.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bmg.bbcook.cn

Ruby: def to_s; @name; end
来源：http://wpx.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://tit.hfpthk.cn

[G13] 判断对象类型
来源：http://ido.bjfxy.top

Py:   isinstance(u, User)
来源：http://edo.cqqwz.cn

PHP:  $u instanceof User
来源：http://tqc.yonumen.top

JS:   u instanceof User
来源：http://vwc.cashguo.top

TS:   u instanceof User
来源：http://uuw.xuetiantiany.cn

Java: u instanceof User
来源：http://sbd.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bqz.zycfv.cn

Ruby: u.is_a?(User)
来源：http://czj.shanyushiyangtech.top

C#:   u is User
来源：http://hyv.ppjwa.cn

[G14] 数据类 / record
来源：http://zhc.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kwe.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://ced.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://sxo.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://kxz.bbcook.cn

Java: record User(String name, int age) {}
来源：http://sjo.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://tqd.zhixingplan.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yvf.yangfankeji.com

C#:   record User(string Name, int Age);
来源：http://grt.quarkkingdee.top

[G15] 枚举
来源：http://ysl.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lku.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zjp.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qvm.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wbx.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://lug.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zjc.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://snk.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bpj.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://ckh.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://han.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://ejm.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://yag.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://ioy.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oak.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://svi.shuidangran.top

Ruby: obj.instance_variables
来源：http://gtr.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://xcq.tanke756.top

================================================================================
来源：http://rex.hnxiangtu.top

H. 异常与错误处理
来源：http://hec.fengsongda.top

================================================================================
来源：http://bds.andypj.xyz

[H01] try / catch 基础
来源：http://ojo.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ofd.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xez.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rar.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gjo.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wxq.yongpay.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://krm.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ncs.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vmp.yj20258888.top

[H02] finally / ensure 收尾
来源：http://ove.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mgk.hesvh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pkv.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ifp.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fec.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://vmn.vqdsnc.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gti.zycfv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://exe.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://grl.fzhhl.top

[H03] 主动抛出异常
来源：http://iod.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://sje.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eqx.9152youxi.cn

JS:   throw new Error("错误信息");
来源：http://leg.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://tdd.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://pmc.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://piy.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fnl.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://fzy.ybcxt.top

[H04] 自定义异常类型
来源：http://xxe.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://gqx.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://ymu.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://tev.yongpay.top

TS:   class MyError extends Error {}
来源：http://hax.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://fud.chenlongwang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hzf.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://tiq.sweek.top

C#:   class MyException : Exception {}
来源：http://kwx.hongshengwenyu.top

[H05] 捕获特定类型
来源：http://lpn.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://qzb.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qjg.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://btz.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://scs.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://lzl.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://shm.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://rlm.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iki.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://hax.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://rhj.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://omq.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://bzj.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://pzr.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fco.dashuyun.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://foy.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://dsw.jiagoushi.top

C#:   obj?.A?.B ?? default
来源：http://iwy.gzhubu.top

[H07] 断言
来源：http://ued.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://lxp.havefunace.top

PHP:  assert($x > 0);
来源：http://lyx.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://zri.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://jdp.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://kmd.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nge.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zue.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://spe.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://tek.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://bwf.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://klc.epnwcf.com

JS:   e.message;  e.stack
来源：http://sqn.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lzs.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://edw.feifeiyinyue.top

Go:   err.Error()
来源：http://hia.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://ohn.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://lrc.aizwys.cn

[H09] 带错误码的异常
来源：http://zxx.xuanzx.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rlc.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vfm.iojbl.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kic.wangshuangyany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lly.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yvc.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fzy.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://bjp.zhixingplan.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cpn.jqgfzy.top

[H10] 资源自动释放
来源：http://wmg.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qak.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xyq.0kj1m.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wzm.ppjwa.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rcl.cucudq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vtc.snrcjt.cn

Go:   defer f.Close()
来源：http://foi.hfpthk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pta.cheryme.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xyb.xziqi.cn

================================================================================
来源：http://isb.cqqwz.cn

I. 正则表达式
来源：http://sca.jianghu66.top

================================================================================
来源：http://pls.cqqwz.cn

[I01] 判断是否匹配
来源：http://dyn.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oyo.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pcp.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://fez.cucudq.cn

TS:   /\d+/.test(s)
来源：http://ggz.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://icj.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oag.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://cpr.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pjz.tian-w.cn

[I02] 提取所有匹配
来源：http://ekl.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://wey.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bzz.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yon.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://tfc.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gxq.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xgz.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://kro.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ndb.hnxiangtu.top

[I03] 提取捕获分组
来源：http://sfx.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xyz.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xwc.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vpi.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ypq.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gzy.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zwi.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://utc.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gbq.sweek.top

[I04] 正则替换
来源：http://bmx.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://esw.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cbv.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://idy.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://wfu.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://brc.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eht.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pqc.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://chi.feifeiyinyue.top

[I05] 按正则拆分
来源：http://tst.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://oeo.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zwz.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://uql.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://woo.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://yyi.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kpc.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://qmr.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cwi.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://psq.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gjd.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dgh.ehwqpu.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yci.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpy.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sug.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ycc.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lnp.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sjv.wangdashe.top

[I07] 忽略大小写与多行模式
来源：http://vld.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eoy.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ilo.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://acg.fanxiaobao.xyz

TS:   /error/gim
来源：http://xyi.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tja.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qmo.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://hpv.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rfy.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://oer.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hik.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nxk.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fwr.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jnc.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ziq.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hfg.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xgj.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lai.shangyingyoupin.top

================================================================================
来源：http://qgb.fzhhl.top

J. 日期与时间
来源：http://uyw.cdnleiting.top

================================================================================
来源：http://xow.hongshengwenyu.top

[J01] 获取当前时间
来源：http://zge.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://trw.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uaa.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://xbv.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://lon.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hnk.sjlbkw.cn

Go:   time.Now()
来源：http://suq.vqdsnc.cn

Ruby: Time.now
来源：http://jxu.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://prv.guowangkeji.top

[J02] 格式化输出
来源：http://beh.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yte.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://scx.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ido.shzxlz.cn

TS:   d.toISOString()
来源：http://vgx.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xtb.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ijg.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gmg.shanyushiyangtech.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vyc.sysykeji.top

[J03] 字符串解析为日期
来源：http://vgb.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://opi.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qbo.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://mws.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://rio.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://oht.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xkc.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://cnx.epnwcf.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fza.meibo888.top

[J04] 时间戳与日期互转
来源：http://ozt.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yep.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kld.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ejr.ywan-chungtsiang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ufm.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ivx.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yfu.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://krd.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://azp.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://bsj.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://qjx.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://axy.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://otp.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zzk.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://ftw.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ttj.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://rue.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://gyy.yangfankeji.com

[J06] 计算两时间之差
来源：http://ils.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://wvj.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://cdy.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tmu.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rop.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sbe.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://eek.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://cqh.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://zzq.bbcook.cn

[J07] 比较两个日期
来源：http://epd.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://gzj.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jew.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://zjl.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://auw.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tyy.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qah.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://mkd.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://zmy.bbcook.cn

[J08] 提取年月日与星期
来源：http://tlc.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xec.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gwz.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rin.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dxy.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ouv.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wsr.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mkj.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xhl.feifeiyinyue.top

[J09] 时区处理
来源：http://ktf.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pvf.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://akw.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qtv.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbd.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kjr.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pzf.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ufa.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://amg.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://vmw.gotoacloud.top


<!-- 参考信息 -->