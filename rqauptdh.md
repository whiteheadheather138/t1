代发 wailian999

[Q78] 当前时间
来源：http://ppl.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sfh.smart0.xyz

[Q79] 字符串拼接
来源：http://urk.sxryk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dgy.aizwys.cn

[Q80] 字符串截取
来源：http://eui.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://irw.yueranfly.top

[Q81] 字符串替换
来源：http://ofd.hongshengwenyu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bpo.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://rhl.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fip.cheryme.top

[Q83] 大小写转换
来源：http://yvb.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://puc.tianlin.xyz

[Q84] 去除首尾空格
来源：http://klj.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://sqy.0kj1m.cn

[Q85] 数值取整
来源：http://kgo.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vlu.shanyushiyangkeji.top

[Q86] 读取 JSON 字段
来源：http://zxs.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fbi.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://xaq.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fxs.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://pko.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://quh.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vno.hywenlv.cn

[Q89] 判断表是否存在
来源：http://iyq.yfazqb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tjd.jinqigfzy.top

[Q90] 生成序号列
来源：http://tmp.fengsongda.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://caa.jyoumei.cn

================================================================================
来源：http://jxu.xinyue.icu

R. Bash 专题
来源：http://ral.ywan-chungtsiang.top

================================================================================
来源：http://fum.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://hgw.cdnleiting.top

#!/usr/bin/env bash
来源：http://jvi.gaohongyu789.top

set -euo pipefail
来源：http://uki.xziqi.cn

[R02] 变量赋值与使用
来源：http://zxy.xuetiantiany.cn

name="Tom"; echo "$name"
来源：http://rmp.jinghuilouyu.cn

[R03] 只读变量
来源：http://muh.ppjwa.cn

readonly PI=3.14
来源：http://jvd.cheryme.top

[R04] 位置参数
来源：http://gqe.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zjj.shuidangran.top

[R05] 参数默认值
来源：http://mge.dianchejie.cn

name="${1:-default}"
来源：http://enm.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://tou.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sma.jinqigufen.top

[R07] if 判断文件
来源：http://unt.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lls.fengsongda.top

[R08] 数值比较
来源：http://bam.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iqt.redwolf501.top

[R09] 字符串比较
来源：http://dqy.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://szd.hfpthk.cn

[R10] 正则匹配
来源：http://umc.jiagoushi.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uhw.fzhhl.top

[R11] case 多分支
来源：http://ckn.0kj1m.cn

case "$1" in
来源：http://rzt.ybcxt.top

start) echo "启动" ;;
来源：http://ncw.ppjwa.cn

stop)  echo "停止" ;;
来源：http://ask.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://fvw.hongshengwenyu.top

esac
来源：http://jsj.smart0.xyz

[R12] for 遍历文件
来源：http://khg.hesvh.cn

for f in *.txt; do echo "$f"; done
来源：http://fhi.kuanghao11.cn

[R13] for 计数循环
来源：http://ntg.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://vgr.chenjidiqi.icu

[R14] C 风格 for
来源：http://dcu.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kfa.sweek.top

[R15] while 逐行读文件
来源：http://ojr.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://psl.havefunace.top

[R16] until 等待条件
来源：http://yyh.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bin.vehdjk.com

[R17] 数组定义与取值
来源：http://oft.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://vtr.daxiang520.top

[R18] 遍历数组
来源：http://xei.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://adv.zhaomingkeji.xyz

[R19] 数组长度
来源：http://gjg.jqgufenzy.top

echo "${#arr[@]}"
来源：http://rxg.zhongyouzk.top

[R20] 关联数组（字典）
来源：http://ksx.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ydq.haohaochexian.top

[R21] 字符串长度
来源：http://znm.cheryme.top

echo "${#s}"
来源：http://lgw.hcnkem.com

[R22] 截取子串
来源：http://qsk.andypj.xyz

echo "${s:0:5}"
来源：http://lmb.cheryme.top

[R23] 字符串替换
来源：http://mws.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bms.cucudq.cn

[R24] 大小写转换
来源：http://raz.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://eda.hammf.cn

[R25] 去后缀 / 去前缀
来源：http://imd.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lir.yonumen.top

[R26] 命令替换
来源：http://bpn.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://nte.hysaishi.cn

[R27] 算术展开
来源：http://swg.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://nss.jqgufenzy.top

[R28] 浮点运算
来源：http://bxb.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://wcu.tian-w.cn

[R29] 定义函数
来源：http://tpu.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cqc.hywenlv.cn

[R30] 函数返回状态码
来源：http://yie.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://upx.xziqi.cn

[R31] 局部变量
来源：http://hey.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://fpi.cashguo.top

[R32] 参数个数校验
来源：http://iha.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ekn.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://bkw.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kbj.ehwqpu.com

[R34] 退出时清理
来源：http://jse.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://gut.zdqjudy.top

[R35] 后台执行并等待
来源：http://elm.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nxg.yuanzhike.top

[R36] 并发执行多个任务
来源：http://xql.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bmr.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://ykr.ehwqpu.com

files=$(ls -1)
来源：http://yil.hywenlv.cn

[R38] 管道串联
来源：http://iid.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://mib.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://anf.ydjk.org.cn

cmd > out.log 2>&1
来源：http://ung.zycfv.cn

[R40] 追加写日志
来源：http://muo.sysykeji.top

echo "log" >> out.log
来源：http://dta.redwolf501.top

[R41] 丢弃输出
来源：http://jxm.mhx1999.top

cmd >/dev/null 2>&1
来源：http://esw.zhijiandao.cn

[R42] 输入重定向
来源：http://xyg.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://lpx.chenzaomai.com

[R43] 按名字查找文件
来源：http://fqe.ydjk.org.cn

find . -name "*.log" -type f
来源：http://maf.shzxlz.cn

[R44] 按修改时间查找
来源：http://vok.tianlin.xyz

find . -mtime -7 -type f
来源：http://mdf.316326.xyz

[R45] 批量删除
来源：http://dgb.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://cfi.tarul.cn

[R46] 递归替换文件内容
来源：http://iyt.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rjd.dashuyun.cn

[R47] sed 单行替换
来源：http://kgq.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://aue.guowangkeji.top

[R48] awk 取指定列
来源：http://gqm.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://igp.fanxiaobao.xyz

[R49] awk 带条件
来源：http://ylf.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://doo.hcnkem.com

[R50] awk 求和
来源：http://bnj.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://ddy.hfpthk.cn

[R51] 排序去重取前几
来源：http://she.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dak.hysaishi.cn

[R52] 统计行数
来源：http://yyt.zdbjq.cn

wc -l a.txt
来源：http://eyp.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://ghh.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ske.jlsjyb.cn

[R54] 比较两个文件
来源：http://kxx.jinqigufen.top

diff a.txt b.txt
来源：http://hwz.9152youxi.cn

[R55] 压缩与解压
来源：http://rgg.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://elb.sysykeji.top

[R56] 远程拷贝
来源：http://ykd.jqgfzy.top

scp file user@host:/path/
来源：http://siu.zhijiandao.cn

[R57] 远程执行命令
来源：http://nje.yangfankeji.com

ssh user@host 'uptime'
来源：http://txo.yfazqb.com

[R58] 下载文件
来源：http://iiz.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mpx.mhx1999.top

[R59] 发 POST JSON
来源：http://fof.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vwg.zhaomingkeji.xyz

[R60] 只看 HTTP 状态码
来源：http://xnc.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://adw.fktsv.cn

[R61] 磁盘占用
来源：http://khm.fehbvm.com

df -h;  du -sh *
来源：http://jkx.hesvh.cn

[R62] 找最占空间的文件
来源：http://hqj.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://vyv.sjlbkw.cn

[R63] 内存与进程
来源：http://sty.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://uld.jqgfzy.top

[R64] 结束进程
来源：http://kbq.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://vev.gzhubu.top

[R65] 查看端口占用
来源：http://cws.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qdm.yangfankeji.com

[R66] 定时任务
来源：http://yxr.zhoulong.xyz

crontab -e;  crontab -l
来源：http://mwa.yueranfly.top

[R67] 生成随机十六进制串
来源：http://vzb.jinghuilouyu.cn

openssl rand -hex 16
来源：http://ayr.redwolf501.top

[R68] 计算文件校验值
来源：http://vwr.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://hbn.yvedp.cn

[R69] 生成随机密码
来源：http://mmh.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://dii.yvedp.cn

[R70] 时间戳与互转
来源：http://tqh.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://rqx.ctjpmb.com

[R71] 日期格式化
来源：http://xrv.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://foh.pycfn.com

[R72] 等待端口就绪
来源：http://nzz.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dyb.yuxming.cn

[R73] 分割大日志
来源：http://ezb.sweek.top

split -l 1000 big.log part_
来源：http://bxd.shangyingyoupin.top

[R74] 批量重命名
来源：http://nuj.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://icv.yanxiufei.cn

[R75] 导出环境变量
来源：http://ysc.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://swr.shuidangran.top

[R76] 使用临时文件
来源：http://kdq.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ypj.vehdjk.com

[R77] 读取用户输入
来源：http://nls.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://kdj.bbcook.cn

[R78] 交互式菜单
来源：http://zaz.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vkp.ydzc1.top

[R79] 解析命令行选项
来源：http://qpr.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tas.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://jwh.yj202588.top

time ./run.sh
来源：http://cxt.ybcxt.top

================================================================================
来源：http://dhw.ybcxt.top

S. C / C++ 专题
来源：http://iux.shanyushiyangkeji.top

================================================================================
来源：http://wtw.ybcxt.top

[S01] C：Hello World
来源：http://ppg.cheryme.top

#include <stdio.h>
来源：http://zgz.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fic.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://efe.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://pix.yueranfly.top

[S03] C：读入整数
来源：http://pkf.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://okc.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://dfq.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://bou.ybcxt.top

[S05] C：字符串长度
来源：http://syi.fanxiaobao.xyz

strlen(s)
来源：http://ovk.yueranfly.top

[S06] C：字符串比较
来源：http://ash.zycfv.cn

strcmp(a, b) == 0
来源：http://khq.zdqjudy.top

[S07] C：数组遍历求和
来源：http://kia.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://doe.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://lii.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hnb.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://mkv.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eis.jiagoushi.top

[S10] C：指针与解引用
来源：http://caj.fehbvm.com

int *p = &a;  *p = 5;
来源：http://rcg.hammf.cn

[S11] C：逐行读文件
来源：http://jic.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://lfr.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rhd.tanke756.top

fclose(f);
来源：http://crm.bjfxy.top

[S12] C：写文件
来源：http://ela.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uih.bbcook.cn

[S13] C：宏定义
来源：http://kat.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cgf.shanyushiyangkeji.top

[S14] C：枚举
来源：http://wzj.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://eyw.aizwys.cn

[S15] C：类型转换
来源：http://jec.chenjidiqi.icu

(double) a / b
来源：http://iym.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://icf.shangyingyoupin.top

x |= (1 << 3);
来源：http://lxn.xuetiantiany.cn

[S17] C：安全拼接字符串
来源：http://cbq.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xns.zhongyouzk.top

[S18] C：命令行参数
来源：http://uxd.xinyue.icu

int main(int argc, char **argv)
来源：http://bcj.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://iub.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pdc.ctjpmb.com

[S20] C：二分查找
来源：http://ntg.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wjx.kuanghao11.cn

[S21] C：字符类别判断
来源：http://foi.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uxu.ppjwa.cn

[S22] C：字符串转数字
来源：http://eft.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://hdt.snrcjt.cn

[S23] C：随机数
来源：http://fxr.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://abx.kuanghao11.cn

[S24] C：获取本地时间
来源：http://qpd.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nno.yj20258888.top

[S25] C：内存拷贝
来源：http://vel.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://umh.hnxiangtu.top

[S26] C：内存清零
来源：http://hhx.nwbrower.top

memset(a, 0, sizeof a);
来源：http://civ.yonumen.top

[S27] C：定义常量
来源：http://buo.hfpthk.cn

const double PI = 3.14159;
来源：http://ckb.hongshengwenyu.top

[S28] C：静态变量
来源：http://zgx.jiagoushi.top

static int counter = 0;
来源：http://gwc.guowangkeji.top

[S29] C：变参函数
来源：http://xna.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dfg.uphjek.com

[S30] C：头文件保护
来源：http://ttq.nanxuanxn.top

#ifndef X_H
来源：http://hyo.yangfankeji.com

#define X_H
来源：http://dry.tanke756.top

#endif
来源：http://duc.hywenlv.cn

[S31] C++：Hello World
来源：http://ahe.vehdjk.com

#include <iostream>
来源：http://wim.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://mfp.nanxuanxn.top

[S32] C++：字符串
来源：http://wfx.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://cqw.gogol.net.cn

[S33] C++：vector 增删
来源：http://mry.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kpc.0kj1m.cn

[S34] C++：遍历 vector
来源：http://oxw.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://wtf.fehbvm.com

[S35] C++：map
来源：http://gyc.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kep.sufxvd.cn

[S36] C++：unordered_map
来源：http://jcw.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iqz.cucudq.cn

[S37] C++：set
来源：http://thg.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ktc.aizwys.cn

[S38] C++：排序
来源：http://ave.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://hqj.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://yph.c1oappe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://edv.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://duq.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tki.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://vgt.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vng.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://oqu.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://min.c1oappe.top

[S43] C++：智能指针
来源：http://grz.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://wds.havefunace.top

[S44] C++：引用传参
来源：http://ddm.yuxming.cn

void inc(int &x) { ++x; }
来源：http://fjl.hongshengwenyu.top

[S45] C++：lambda
来源：http://aot.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ubn.xziqi.cn

[S46] C++：函数模板
来源：http://uhg.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hrx.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://uwm.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oyg.havefunace.top

[S48] C++：逐行读文件
来源：http://nwa.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sbn.xinyue.icu


<!-- 参考信息 -->