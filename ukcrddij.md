代发 wailian999

[Q78] 当前时间
来源：http://rcr.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wpy.fengsongda.top

[Q79] 字符串拼接
来源：http://tpi.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lzq.sysykeji.top

[Q80] 字符串截取
来源：http://vfp.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eyr.yj20258888.top

[Q81] 字符串替换
来源：http://gqe.fanxiaobao.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bmq.yj20258888.top

[Q82] 字符长度与字节长度
来源：http://cbz.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dzw.yj20258.top

[Q83] 大小写转换
来源：http://slz.ydjk.org.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qfj.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://xir.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://qcm.daxiang520.top

[Q85] 数值取整
来源：http://uig.zhiwuduotai.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ypr.cdnleiting.top

[Q86] 读取 JSON 字段
来源：http://fnj.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dfg.hammf.cn

[Q87] JSON 字段做条件
来源：http://xhx.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wta.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://xdq.gotoacloud.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wbn.zhongyouzk.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tfv.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://vbu.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yah.ydzc1.top

[Q90] 生成序号列
来源：http://otd.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vot.hcnkem.com

================================================================================
来源：http://hrd.gzhubu.top

R. Bash 专题
来源：http://akv.andypj.xyz

================================================================================
来源：http://jjs.hywenlv.cn

[R01] shebang 与严格模式
来源：http://smh.aizwys.cn

#!/usr/bin/env bash
来源：http://zts.fengsongda.top

set -euo pipefail
来源：http://vzf.fktsv.cn

[R02] 变量赋值与使用
来源：http://dlh.dashuyun.cn

name="Tom"; echo "$name"
来源：http://cdr.hongshengwenyu.top

[R03] 只读变量
来源：http://aqb.tarul.cn

readonly PI=3.14
来源：http://fit.zhoulong.xyz

[R04] 位置参数
来源：http://pqg.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iid.snrcjt.cn

[R05] 参数默认值
来源：http://oai.jqgufenzy.top

name="${1:-default}"
来源：http://emy.gotoacloud.top

[R06] 判断命令是否存在
来源：http://osh.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iyr.daxiang520.top

[R07] if 判断文件
来源：http://buw.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gsg.vehdjk.com

[R08] 数值比较
来源：http://gla.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lgb.tarul.cn

[R09] 字符串比较
来源：http://jyh.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://otw.chenzaomai.com

[R10] 正则匹配
来源：http://kvs.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nyi.shangyingyoupin.top

[R11] case 多分支
来源：http://oip.dashuyun.cn

case "$1" in
来源：http://eab.zhijiandao.cn

start) echo "启动" ;;
来源：http://xni.xinyue.icu

stop)  echo "停止" ;;
来源：http://hie.smart0.xyz

*)     echo "未知命令" ;;
来源：http://sgl.zhoulong.xyz

esac
来源：http://sht.gotoacloud.top

[R12] for 遍历文件
来源：http://usr.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://cqj.ydjk.org.cn

[R13] for 计数循环
来源：http://iga.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://rtz.quarkkingdee.top

[R14] C 风格 for
来源：http://dyl.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ifv.zhixingplan.top

[R15] while 逐行读文件
来源：http://ele.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xsy.andypj.xyz

[R16] until 等待条件
来源：http://jdy.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://msl.yongpay.top

[R17] 数组定义与取值
来源：http://jzn.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://yac.daria6918.cn

[R18] 遍历数组
来源：http://htx.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ggt.mhx1999.top

[R19] 数组长度
来源：http://gzo.svipenyu.cn

echo "${#arr[@]}"
来源：http://wuk.sysykeji.top

[R20] 关联数组（字典）
来源：http://gmy.jinqigfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sws.yongpay.top

[R21] 字符串长度
来源：http://btw.yvedp.cn

echo "${#s}"
来源：http://pey.hongshengwenyu.top

[R22] 截取子串
来源：http://dtr.hcnkem.com

echo "${s:0:5}"
来源：http://igo.yfazqb.com

[R23] 字符串替换
来源：http://jnk.quarkkingdee.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xbk.pycfn.com

[R24] 大小写转换
来源：http://eke.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xfa.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://wqn.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fcc.redwolf501.top

[R26] 命令替换
来源：http://gcc.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://xwy.0kj1m.cn

[R27] 算术展开
来源：http://pwl.vehdjk.com

echo $((1 + 2 * 3))
来源：http://mfh.ydjk.org.cn

[R28] 浮点运算
来源：http://vjd.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://cmk.hfpthk.cn

[R29] 定义函数
来源：http://svc.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zud.c1oappe.top

[R30] 函数返回状态码
来源：http://hhq.jyoumei.cn

f() { return 0; }; f || echo "失败了"
来源：http://gmq.ctjpmb.com

[R31] 局部变量
来源：http://pjf.zhoulong.xyz

f() { local x=1; echo "$x"; }
来源：http://nkl.xinyue.icu

[R32] 参数个数校验
来源：http://uod.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kak.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://vlh.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lzm.ydjk.org.cn

[R34] 退出时清理
来源：http://ktn.hesvh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oze.zhongyouzk.top

[R35] 后台执行并等待
来源：http://lks.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zlh.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://anq.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yze.birdmap.top

[R37] 把输出赋给变量
来源：http://dru.hammf.cn

files=$(ls -1)
来源：http://wvp.xylfe.cn

[R38] 管道串联
来源：http://unm.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://cat.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://lkp.guannengcc.top

cmd > out.log 2>&1
来源：http://kjo.sufxvd.cn

[R40] 追加写日志
来源：http://wwe.cqqwz.cn

echo "log" >> out.log
来源：http://gta.uphjek.com

[R41] 丢弃输出
来源：http://duj.vehdjk.com

cmd >/dev/null 2>&1
来源：http://rlc.vqdsnc.cn

[R42] 输入重定向
来源：http://pfp.jinqigfzy.top

wc -l < a.txt
来源：http://irw.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://enj.redwolf501.top

find . -name "*.log" -type f
来源：http://ghb.hammf.cn

[R44] 按修改时间查找
来源：http://eua.c1oappe.top

find . -mtime -7 -type f
来源：http://njv.ydjk.org.cn

[R45] 批量删除
来源：http://enx.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://ktf.ivvv.top

[R46] 递归替换文件内容
来源：http://bxd.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bnq.nanxuanxn.top

[R47] sed 单行替换
来源：http://zwk.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://mjy.shangyingyoupin.top

[R48] awk 取指定列
来源：http://dah.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://mja.tarul.cn

[R49] awk 带条件
来源：http://yoc.jinqigfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sgo.ywan-chungtsiang.top

[R50] awk 求和
来源：http://iky.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qjh.yj202588.top

[R51] 排序去重取前几
来源：http://nan.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bqq.yangfankeji.com

[R52] 统计行数
来源：http://ewm.fanxiaobao.xyz

wc -l a.txt
来源：http://pvx.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://zrq.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vra.xuetiantiany.cn

[R54] 比较两个文件
来源：http://njb.snrcjt.cn

diff a.txt b.txt
来源：http://vuv.cashguo.top

[R55] 压缩与解压
来源：http://jwf.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tir.52xcode.cn

[R56] 远程拷贝
来源：http://keq.yonumen.top

scp file user@host:/path/
来源：http://bpm.yangfankeji.com

[R57] 远程执行命令
来源：http://xet.yuxming.cn

ssh user@host 'uptime'
来源：http://zql.ctjpmb.com

[R58] 下载文件
来源：http://wym.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qul.jyoumei.cn

[R59] 发 POST JSON
来源：http://xod.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ldj.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://wjx.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ich.fzhhl.top

[R61] 磁盘占用
来源：http://fkm.smart0.xyz

df -h;  du -sh *
来源：http://wuv.gotoacloud.top

[R62] 找最占空间的文件
来源：http://ifi.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://hqn.ctjpmb.com

[R63] 内存与进程
来源：http://jlp.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://ijd.tarul.cn

[R64] 结束进程
来源：http://vzs.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://tmd.jyoumei.cn

[R65] 查看端口占用
来源：http://oel.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdr.jiagoushi.top

[R66] 定时任务
来源：http://lnl.ivvv.top

crontab -e;  crontab -l
来源：http://ews.ivvv.top

[R67] 生成随机十六进制串
来源：http://rjp.jinqigfzy.top

openssl rand -hex 16
来源：http://lwd.uphjek.com

[R68] 计算文件校验值
来源：http://vvg.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nsq.yj20258888.top

[R69] 生成随机密码
来源：http://lab.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://sif.yongpay.top

[R70] 时间戳与互转
来源：http://eae.hcnkem.com

date +%s;  date -d @1700000000
来源：http://gzw.jinqigufen.top

[R71] 日期格式化
来源：http://dnw.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://tbr.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://rrw.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fxf.feifeiyinyue.top

[R73] 分割大日志
来源：http://vuk.chenzaomai.com

split -l 1000 big.log part_
来源：http://kfk.hywenlv.cn

[R74] 批量重命名
来源：http://kom.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qpl.andypj.xyz

[R75] 导出环境变量
来源：http://iio.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://nwi.yonumen.top

[R76] 使用临时文件
来源：http://fub.tian-w.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tzj.aizwys.cn

[R77] 读取用户输入
来源：http://spz.dashuyun.cn

read -rp "请输入: " ans
来源：http://yef.zycfv.cn

[R78] 交互式菜单
来源：http://pgd.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rtk.jinqigufen.top

[R79] 解析命令行选项
来源：http://ijz.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zbt.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://bgo.pycfn.com

time ./run.sh
来源：http://pbx.hcnkem.com

================================================================================
来源：http://bzn.52xcode.cn

S. C / C++ 专题
来源：http://ygs.aibaodan.cn

================================================================================
来源：http://zhb.zhongyouzk.top

[S01] C：Hello World
来源：http://uih.yfazqb.com

#include <stdio.h>
来源：http://qou.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://afi.yvedp.cn

[S02] C：变量与格式化输出
来源：http://drk.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://smm.zhiwuduotai.top

[S03] C：读入整数
来源：http://xkl.zhengqikj.top

int x; scanf("%d", &x);
来源：http://nfk.chenjidiqi.icu

[S04] C：字符串复制
来源：http://rbi.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://agp.hnqzz.top

[S05] C：字符串长度
来源：http://ahl.yangfankeji.com

strlen(s)
来源：http://hsk.hfpthk.cn

[S06] C：字符串比较
来源：http://jto.hammf.cn

strcmp(a, b) == 0
来源：http://vlw.mhx1999.top

[S07] C：数组遍历求和
来源：http://eud.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pya.shzxlz.cn

[S08] C：动态内存分配与释放
来源：http://qoi.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dsq.sweek.top

[S09] C：结构体定义与初始化
来源：http://vdr.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://awm.316326.xyz

[S10] C：指针与解引用
来源：http://txy.birdmap.top

int *p = &a;  *p = 5;
来源：http://tqu.shuidangran.top

[S11] C：逐行读文件
来源：http://wzc.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://tcn.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://nqm.ehwqpu.com

fclose(f);
来源：http://fsh.zdqjudy.top

[S12] C：写文件
来源：http://gzh.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tcy.yj20258.top

[S13] C：宏定义
来源：http://aow.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://diu.jiagoushi.top

[S14] C：枚举
来源：http://rrt.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://mzg.52xcode.cn

[S15] C：类型转换
来源：http://rai.sxryk.cn

(double) a / b
来源：http://ica.hesvh.cn

[S16] C：位操作置位
来源：http://kzm.xuanzx.com

x |= (1 << 3);
来源：http://fve.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://bca.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ixr.hnqzz.top

[S18] C：命令行参数
来源：http://cpi.vehdjk.com

int main(int argc, char **argv)
来源：http://hhz.havefunace.top

[S19] C：快速排序
来源：http://cpa.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ive.yanxiufei.cn

[S20] C：二分查找
来源：http://zth.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mch.zycfv.cn

[S21] C：字符类别判断
来源：http://bkm.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://klp.quarkkingdee.top

[S22] C：字符串转数字
来源：http://inq.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fiw.zhaomingkeji.xyz

[S23] C：随机数
来源：http://vxg.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://mzw.haohaochexian.top

[S24] C：获取本地时间
来源：http://zhc.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bbd.vehdjk.com

[S25] C：内存拷贝
来源：http://uje.kuanghao11.cn

memcpy(dst, src, n);
来源：http://kxy.cdnleiting.top

[S26] C：内存清零
来源：http://grb.xziqi.cn

memset(a, 0, sizeof a);
来源：http://pym.bbcook.cn

[S27] C：定义常量
来源：http://eoe.yfazqb.com

const double PI = 3.14159;
来源：http://axj.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://mgn.xingfuxueyuan.xyz

static int counter = 0;
来源：http://pib.gotoacloud.top

[S29] C：变参函数
来源：http://ryd.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hrw.316326.xyz

[S30] C：头文件保护
来源：http://oei.yongpay.top

#ifndef X_H
来源：http://lbq.bjfxy.top

#define X_H
来源：http://hrb.jiagoushi.top

#endif
来源：http://oxt.cqqwz.cn

[S31] C++：Hello World
来源：http://fol.dashuyun.cn

#include <iostream>
来源：http://yfh.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://ifj.yanxiufei.cn

[S32] C++：字符串
来源：http://itk.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://ptk.xziqi.cn

[S33] C++：vector 增删
来源：http://agi.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cts.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://mhd.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://ewe.meibo888.top

[S35] C++：map
来源：http://qlg.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://glm.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://iuz.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tvj.jinyuanbaomall.cn

[S37] C++：set
来源：http://czs.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ohn.aizwys.cn

[S38] C++：排序
来源：http://lhm.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://oyr.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://rww.smart0.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rev.jlsjyb.cn

[S40] C++：查找元素
来源：http://sfh.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nvu.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://bnu.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gop.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://vqf.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://rpv.fehbvm.com

[S43] C++：智能指针
来源：http://iqq.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://udy.sysykeji.top

[S44] C++：引用传参
来源：http://zon.yonumen.top

void inc(int &x) { ++x; }
来源：http://usq.zycfv.cn

[S45] C++：lambda
来源：http://mfv.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://wsj.zdqjudy.top

[S46] C++：函数模板
来源：http://ain.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xup.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://rcq.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aao.cucudq.cn

[S48] C++：逐行读文件
来源：http://ffh.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ypb.sweek.top


<!-- 参考信息 -->