代发 wailian999

[Q80] 字符串截取
来源：http://wdn.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ems.dashuyun.cn

[Q81] 字符串替换
来源：http://zrl.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gou.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://zbc.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ehh.daria6918.cn

[Q83] 大小写转换
来源：http://mix.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zbj.chenlongwang.top

[Q84] 去除首尾空格
来源：http://oua.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://xoy.ivvv.top

[Q85] 数值取整
来源：http://elh.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pri.havefunace.top

[Q86] 读取 JSON 字段
来源：http://smg.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mim.yj20258888.top

[Q87] JSON 字段做条件
来源：http://pxn.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ifg.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://cxf.birdmap.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qib.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bey.xuanzx.com

[Q89] 判断表是否存在
来源：http://rqf.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wtv.shanyushiyangtech.top

[Q90] 生成序号列
来源：http://zax.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cae.yvedp.cn

================================================================================
来源：http://znx.meibo888.top

R. Bash 专题
来源：http://khx.316326.xyz

================================================================================
来源：http://bvs.tanke756.top

[R01] shebang 与严格模式
来源：http://qex.smart0.xyz

#!/usr/bin/env bash
来源：http://eso.jinghuilouyu.cn

set -euo pipefail
来源：http://sdr.sweek.top

[R02] 变量赋值与使用
来源：http://rnx.hesvh.cn

name="Tom"; echo "$name"
来源：http://iia.xuetiantiany.cn

[R03] 只读变量
来源：http://mjk.jqgufenzy.top

readonly PI=3.14
来源：http://iti.nanxinkj.top

[R04] 位置参数
来源：http://tvt.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tob.shangyingyoupin.top

[R05] 参数默认值
来源：http://seu.zhijiandao.cn

name="${1:-default}"
来源：http://yfp.xuanzx.com

[R06] 判断命令是否存在
来源：http://qtc.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dbi.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://acl.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uoy.yvedp.cn

[R08] 数值比较
来源：http://fru.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kms.uphjek.com

[R09] 字符串比较
来源：http://azc.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xnj.hysaishi.cn

[R10] 正则匹配
来源：http://hsx.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yus.ywan-chungtsiang.top

[R11] case 多分支
来源：http://mpw.aibaodan.cn

case "$1" in
来源：http://ovt.gogol.net.cn

start) echo "启动" ;;
来源：http://ffa.ydjk.org.cn

stop)  echo "停止" ;;
来源：http://ilz.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://eku.jlsjyb.cn

esac
来源：http://iee.xziqi.cn

[R12] for 遍历文件
来源：http://eqb.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://dgz.meibo888.top

[R13] for 计数循环
来源：http://pcz.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://old.meibo888.top

[R14] C 风格 for
来源：http://czl.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ljw.yueranfly.top

[R15] while 逐行读文件
来源：http://ohd.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uxy.sysykeji.top

[R16] until 等待条件
来源：http://aqj.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fnl.ydjk.org.cn

[R17] 数组定义与取值
来源：http://erp.yongpay.top

arr=(a b c); echo "${arr[0]}"
来源：http://ehi.sufxvd.cn

[R18] 遍历数组
来源：http://jwa.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dbo.ydzc1.top

[R19] 数组长度
来源：http://xli.jlsjyb.cn

echo "${#arr[@]}"
来源：http://uuw.sysykeji.top

[R20] 关联数组（字典）
来源：http://nfc.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ert.xinyue.icu

[R21] 字符串长度
来源：http://siv.xziqi.cn

echo "${#s}"
来源：http://fgx.nwbrower.top

[R22] 截取子串
来源：http://dan.52xcode.cn

echo "${s:0:5}"
来源：http://ziw.jiagoushi.top

[R23] 字符串替换
来源：http://equ.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cks.vehdjk.com

[R24] 大小写转换
来源：http://dru.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://alo.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://hhy.cheryme.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://urb.daria6918.cn

[R26] 命令替换
来源：http://qtp.daxiang520.top

now=$(date +%F); echo "$now"
来源：http://wry.epnwcf.com

[R27] 算术展开
来源：http://sat.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://dxo.aizwys.cn

[R28] 浮点运算
来源：http://iyx.vehdjk.com

echo "scale=2; 10/3" | bc
来源：http://xko.9152youxi.cn

[R29] 定义函数
来源：http://gnz.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zze.wangdashe.top

[R30] 函数返回状态码
来源：http://oyw.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://zlp.meibo888.top

[R31] 局部变量
来源：http://zuh.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://pom.sysykeji.top

[R32] 参数个数校验
来源：http://hyz.havefunace.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nyx.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://plj.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lku.hammf.cn

[R34] 退出时清理
来源：http://jzt.xuanzx.com

trap 'rm -f "$tmp"' EXIT
来源：http://ahv.pycfn.com

[R35] 后台执行并等待
来源：http://qiv.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://bei.gogol.net.cn

[R36] 并发执行多个任务
来源：http://ysk.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sbc.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://pob.0kj1m.cn

files=$(ls -1)
来源：http://gbj.jiagoushi.top

[R38] 管道串联
来源：http://fus.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://gfg.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://jvm.jlsjyb.cn

cmd > out.log 2>&1
来源：http://fxc.fanxiaobao.xyz

[R40] 追加写日志
来源：http://bxo.yuanzhike.top

echo "log" >> out.log
来源：http://zhr.hywenlv.cn

[R41] 丢弃输出
来源：http://wft.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://xve.hnqzz.top

[R42] 输入重定向
来源：http://wko.yvedp.cn

wc -l < a.txt
来源：http://olw.ybcxt.top

[R43] 按名字查找文件
来源：http://aho.hywenlv.cn

find . -name "*.log" -type f
来源：http://iuo.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://tom.fengsongda.top

find . -mtime -7 -type f
来源：http://tyr.cqqwz.cn

[R45] 批量删除
来源：http://jvu.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://omm.fengsongda.top

[R46] 递归替换文件内容
来源：http://vqb.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uem.aizwys.cn

[R47] sed 单行替换
来源：http://qzf.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://emy.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://fcf.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://dzg.hongshengwenyu.top

[R49] awk 带条件
来源：http://jso.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bxh.dianchejie.cn

[R50] awk 求和
来源：http://msv.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://jda.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://jte.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://aes.fktsv.cn

[R52] 统计行数
来源：http://ywr.yonumen.top

wc -l a.txt
来源：http://emy.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://pcj.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ssq.zhongyouzk.top

[R54] 比较两个文件
来源：http://umx.zhixingplan.top

diff a.txt b.txt
来源：http://skh.dianchejie.cn

[R55] 压缩与解压
来源：http://ayj.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xbw.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://gyh.yuanzhike.top

scp file user@host:/path/
来源：http://khx.bbcook.cn

[R57] 远程执行命令
来源：http://wac.zycfv.cn

ssh user@host 'uptime'
来源：http://oyy.jqgufenzy.top

[R58] 下载文件
来源：http://ohs.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xux.dashuyun.cn

[R59] 发 POST JSON
来源：http://crw.sjlbkw.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cdy.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://dgm.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jfl.316326.xyz

[R61] 磁盘占用
来源：http://ekf.haohaochexian.top

df -h;  du -sh *
来源：http://qkv.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://nup.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://qmv.cqqwz.cn

[R63] 内存与进程
来源：http://rom.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://eag.tianlin.xyz

[R64] 结束进程
来源：http://jxp.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://kjc.aibaodan.cn

[R65] 查看端口占用
来源：http://ynw.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qjc.ivvv.top

[R66] 定时任务
来源：http://lvl.zdqjudy.top

crontab -e;  crontab -l
来源：http://osm.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://bqc.sxryk.cn

openssl rand -hex 16
来源：http://bkt.tarul.cn

[R68] 计算文件校验值
来源：http://wal.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dxg.c1oappe.top

[R69] 生成随机密码
来源：http://pkd.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://ans.zhongyouzk.top

[R70] 时间戳与互转
来源：http://rvf.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://fcd.cashguo.top

[R71] 日期格式化
来源：http://pqt.yfazqb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://iao.jinqigfzy.top

[R72] 等待端口就绪
来源：http://fjq.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://fox.jinqigfzy.top

[R73] 分割大日志
来源：http://tmh.hysaishi.cn

split -l 1000 big.log part_
来源：http://wqz.aizwys.cn

[R74] 批量重命名
来源：http://mte.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hiy.fengsongda.top

[R75] 导出环境变量
来源：http://bpp.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://jvn.hcnkem.com

[R76] 使用临时文件
来源：http://rhu.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://twt.zycfv.cn

[R77] 读取用户输入
来源：http://xck.zdqjudy.top

read -rp "请输入: " ans
来源：http://erz.vehdjk.com

[R78] 交互式菜单
来源：http://jbs.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://baa.yj20258.top

[R79] 解析命令行选项
来源：http://pgu.jqgufenzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cim.cheryme.top

[R80] 查看脚本执行耗时
来源：http://wch.bjfxy.top

time ./run.sh
来源：http://ksc.gogol.net.cn

================================================================================
来源：http://kfr.yuxming.cn

S. C / C++ 专题
来源：http://nry.sjlbkw.cn

================================================================================
来源：http://atk.jinqigfzy.top

[S01] C：Hello World
来源：http://sxh.nanxuanxn.top

#include <stdio.h>
来源：http://fqh.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xlc.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://ctt.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://rsv.aizwys.cn

[S03] C：读入整数
来源：http://lse.yongpay.top

int x; scanf("%d", &x);
来源：http://ytl.cqqwz.cn

[S04] C：字符串复制
来源：http://oox.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://jwu.gzhubu.top

[S05] C：字符串长度
来源：http://vkp.cqqwz.cn

strlen(s)
来源：http://jpl.guannengcc.top

[S06] C：字符串比较
来源：http://sar.c1oappe.top

strcmp(a, b) == 0
来源：http://wws.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://uoz.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hje.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://ldq.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tdy.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://ncc.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pxd.vqdsnc.cn

[S10] C：指针与解引用
来源：http://awp.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://ydg.nwbrower.top

[S11] C：逐行读文件
来源：http://scy.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://zck.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ome.zhongyouzk.top

fclose(f);
来源：http://mmt.iojbl.cn

[S12] C：写文件
来源：http://yxm.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rir.xuetiantiany.cn

[S13] C：宏定义
来源：http://gun.yanxiufei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vhg.havefunace.top

[S14] C：枚举
来源：http://dei.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://uqs.yangfankeji.com

[S15] C：类型转换
来源：http://xez.ctjpmb.com

(double) a / b
来源：http://cic.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://yvx.quarkkingdee.top

x |= (1 << 3);
来源：http://mhn.meibo888.top

[S17] C：安全拼接字符串
来源：http://wlw.jinyuanbaomall.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xro.iojbl.cn

[S18] C：命令行参数
来源：http://bbm.fanxiaobao.xyz

int main(int argc, char **argv)
来源：http://urs.chenzaomai.com

[S19] C：快速排序
来源：http://ujd.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ccm.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://lem.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tjw.fehbvm.com

[S21] C：字符类别判断
来源：http://rsk.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gej.yangfankeji.com

[S22] C：字符串转数字
来源：http://gls.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://ios.zhengqikj.top

[S23] C：随机数
来源：http://pxe.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://joc.hesvh.cn

[S24] C：获取本地时间
来源：http://xth.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xzq.aibaodan.cn

[S25] C：内存拷贝
来源：http://uma.nanxuanxn.top

memcpy(dst, src, n);
来源：http://cak.yj202588.top

[S26] C：内存清零
来源：http://xys.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://xvz.xinyue.icu

[S27] C：定义常量
来源：http://vdm.jyoumei.cn

const double PI = 3.14159;
来源：http://ovg.gaohongyu789.top

[S28] C：静态变量
来源：http://ryl.jinqigufen.top

static int counter = 0;
来源：http://avs.dianchejie.cn

[S29] C：变参函数
来源：http://lue.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://guv.hongshengwenyu.top

[S30] C：头文件保护
来源：http://vnh.zhongyouzk.top

#ifndef X_H
来源：http://ceh.tanke756.top

#define X_H
来源：http://gck.vqdsnc.cn

#endif
来源：http://jyd.guannengcc.top

[S31] C++：Hello World
来源：http://eym.zycfv.cn

#include <iostream>
来源：http://jbm.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://xvb.cheryme.top

[S32] C++：字符串
来源：http://dsy.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://wus.hnxiangtu.top

[S33] C++：vector 增删
来源：http://jpm.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://unk.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://krh.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://rhn.hnqzz.top

[S35] C++：map
来源：http://dmp.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xdw.zhiwuduotai.top

[S36] C++：unordered_map
来源：http://gez.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uai.nanxuanxn.top

[S37] C++：set
来源：http://lkp.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://axg.jlsjyb.cn

[S38] C++：排序
来源：http://eua.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://ibg.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://txz.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jma.tanke756.top

[S40] C++：查找元素
来源：http://eom.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yni.ctjpmb.com

[S41] C++：类与构造函数
来源：http://xgw.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lym.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://krv.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://pyy.feifeiyinyue.top

[S43] C++：智能指针
来源：http://ppr.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://bxg.ybcxt.top

[S44] C++：引用传参
来源：http://sea.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://ypx.zdqjudy.top

[S45] C++：lambda
来源：http://udd.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ipb.fengsongda.top

[S46] C++：函数模板
来源：http://wgi.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qat.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://pwj.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xls.zhengqikj.top

[S48] C++：逐行读文件
来源：http://inj.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://zid.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://ary.shuidangran.top

[S49] C++：写文件
来源：http://xci.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yel.nanxinkj.top

[S50] C++：格式化数字
来源：http://uya.yueranfly.top


<!-- 参考信息 -->