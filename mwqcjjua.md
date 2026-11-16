代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lhz.sweek.top

[Q60] 取上一行 / 下一行
来源：http://zrz.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vti.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rik.redwolf501.top

[Q61] 移动平均
来源：http://nmm.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fyx.dianchejie.cn

[Q62] 分组占比
来源：http://trq.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gdm.yangfankeji.com

[Q63] 开启事务
来源：http://qri.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jpo.xinyue.icu

[Q64] 提交事务
来源：http://psv.sysykeji.top

COMMIT;
来源：http://arq.mhx1999.top

[Q65] 回滚事务
来源：http://amt.zycfv.cn

ROLLBACK;
来源：http://dgc.ydjk.org.cn

[Q66] 行锁查询
来源：http://xaa.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cfv.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://hjy.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ksi.zycfv.cn

[Q68] 保存点
来源：http://ago.nanxuanxn.top

SAVEPOINT sp1;
来源：http://mmj.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://vxd.hysaishi.cn

[Q69] 查看执行计划
来源：http://kje.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nnk.tian-w.cn

[Q70] 更新统计信息
来源：http://nqg.chenzaomai.com

ANALYZE TABLE users;
来源：http://cqp.bbcook.cn

[Q71] 查看建表语句
来源：http://rkt.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rrb.zhongyouzk.top

[Q72] 查看索引
来源：http://phf.jinqigfzy.top

SHOW INDEX FROM users;
来源：http://uue.chenzaomai.com

[Q73] 查看表状态
来源：http://xon.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qwj.yueranfly.top

[Q74] 强制使用索引
来源：http://ael.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sln.zhiwuduotai.top

[Q75] 日期格式化
来源：http://lsw.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ckr.guowangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gxe.yangfankeji.com

[Q76] 按天统计
来源：http://tbr.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fsa.quarkkingdee.top

[Q77] 时间加减
来源：http://jic.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://coz.jyoumei.cn

[Q78] 当前时间
来源：http://one.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oal.yonumen.top

[Q79] 字符串拼接
来源：http://xdl.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fut.zdqjudy.top

[Q80] 字符串截取
来源：http://mie.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qab.uphjek.com

[Q81] 字符串替换
来源：http://ypm.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xcc.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://tas.yongpay.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uyj.shangyingyoupin.top

[Q83] 大小写转换
来源：http://khn.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zkx.sufxvd.cn

[Q84] 去除首尾空格
来源：http://gze.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://nhe.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://hvw.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pks.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://uos.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cio.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://qvy.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://imm.jinyuanbaomall.cn

[Q88] 行转列（条件聚合）
来源：http://xsa.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xhf.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lrm.bjfxy.top

[Q89] 判断表是否存在
来源：http://kgl.yj20258888.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ybn.zhixingplan.top

[Q90] 生成序号列
来源：http://rbc.jyoumei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qxl.yvedp.cn

================================================================================
来源：http://dzp.gogol.net.cn

R. Bash 专题
来源：http://iiu.fengsongda.top

================================================================================
来源：http://lvq.cdnleiting.top

[R01] shebang 与严格模式
来源：http://grm.haohaochexian.top

#!/usr/bin/env bash
来源：http://rke.fehbvm.com

set -euo pipefail
来源：http://hxw.hcnkem.com

[R02] 变量赋值与使用
来源：http://omd.dashuyun.cn

name="Tom"; echo "$name"
来源：http://iza.fktsv.cn

[R03] 只读变量
来源：http://dls.wangdashe.top

readonly PI=3.14
来源：http://zsu.tanke756.top

[R04] 位置参数
来源：http://ayl.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cce.tianlin.xyz

[R05] 参数默认值
来源：http://lud.aibaodan.cn

name="${1:-default}"
来源：http://cof.nanxuanxn.top

[R06] 判断命令是否存在
来源：http://txa.tianlin.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://soh.hywenlv.cn

[R07] if 判断文件
来源：http://dxp.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jzi.bjfxy.top

[R08] 数值比较
来源：http://hdk.fktsv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xmi.yueranfly.top

[R09] 字符串比较
来源：http://qed.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kcu.fehbvm.com

[R10] 正则匹配
来源：http://lnc.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ycv.jqgfzy.top

[R11] case 多分支
来源：http://dfm.jinghuilouyu.cn

case "$1" in
来源：http://uyh.zhixingplan.top

start) echo "启动" ;;
来源：http://psm.gogol.net.cn

stop)  echo "停止" ;;
来源：http://lan.yvedp.cn

*)     echo "未知命令" ;;
来源：http://juc.hnqzz.top

esac
来源：http://jyk.yuxming.cn

[R12] for 遍历文件
来源：http://xvh.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://qqm.chenzaomai.com

[R13] for 计数循环
来源：http://vhq.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://djf.daria6918.cn

[R14] C 风格 for
来源：http://aoq.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hnv.chenzaomai.com

[R15] while 逐行读文件
来源：http://mcj.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://irs.cqqwz.cn

[R16] until 等待条件
来源：http://ysc.xziqi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tbl.sysykeji.top

[R17] 数组定义与取值
来源：http://nyi.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://gwd.ehwqpu.com

[R18] 遍历数组
来源：http://yrd.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xhh.yangfankeji.com

[R19] 数组长度
来源：http://riu.fktsv.cn

echo "${#arr[@]}"
来源：http://pwu.yj20258.top

[R20] 关联数组（字典）
来源：http://nyo.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://llz.redwolf501.top

[R21] 字符串长度
来源：http://dat.jiagoushi.top

echo "${#s}"
来源：http://ihq.bjfxy.top

[R22] 截取子串
来源：http://lwj.vehdjk.com

echo "${s:0:5}"
来源：http://oqu.chenzaomai.com

[R23] 字符串替换
来源：http://bxy.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xpg.cdnleiting.top

[R24] 大小写转换
来源：http://vzj.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://wvs.jinqigufen.top

[R25] 去后缀 / 去前缀
来源：http://fkn.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cxe.cucudq.cn

[R26] 命令替换
来源：http://evd.yongpay.top

now=$(date +%F); echo "$now"
来源：http://dgk.yanxiufei.cn

[R27] 算术展开
来源：http://ztl.c1oappe.top

echo $((1 + 2 * 3))
来源：http://iao.dianchejie.cn

[R28] 浮点运算
来源：http://doe.zhiwuduotai.top

echo "scale=2; 10/3" | bc
来源：http://eim.nanxinkj.top

[R29] 定义函数
来源：http://mec.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xvg.iojbl.cn

[R30] 函数返回状态码
来源：http://rqj.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://mlu.nanxinkj.top

[R31] 局部变量
来源：http://swr.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://vvp.zhijiandao.cn

[R32] 参数个数校验
来源：http://emu.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rch.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://rjn.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://anw.hcnkem.com

[R34] 退出时清理
来源：http://zqp.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vli.svipenyu.cn

[R35] 后台执行并等待
来源：http://bru.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://rin.xziqi.cn

[R36] 并发执行多个任务
来源：http://pvz.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://awl.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://pou.yj20258.top

files=$(ls -1)
来源：http://vwj.gotoacloud.top

[R38] 管道串联
来源：http://glt.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://tzn.ydzc1.top

[R39] 重定向标准输出与错误
来源：http://vwz.zhixingplan.top

cmd > out.log 2>&1
来源：http://nii.zdbjq.cn

[R40] 追加写日志
来源：http://vkn.shzxlz.cn

echo "log" >> out.log
来源：http://twc.cheryme.top

[R41] 丢弃输出
来源：http://jwf.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://rdi.bjfxy.top

[R42] 输入重定向
来源：http://uzi.bbcook.cn

wc -l < a.txt
来源：http://jxs.hcnkem.com

[R43] 按名字查找文件
来源：http://kjd.hysaishi.cn

find . -name "*.log" -type f
来源：http://ikp.jinqigfzy.top

[R44] 按修改时间查找
来源：http://sih.xuanzx.com

find . -mtime -7 -type f
来源：http://eau.yj20258.top

[R45] 批量删除
来源：http://xcc.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://bdd.hfpthk.cn

[R46] 递归替换文件内容
来源：http://sam.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yua.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://mnx.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ivl.birdmap.top

[R48] awk 取指定列
来源：http://ugz.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://wqy.xuanzx.com

[R49] awk 带条件
来源：http://tmr.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bds.redwolf501.top

[R50] awk 求和
来源：http://wfl.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://tos.zhoulong.xyz

[R51] 排序去重取前几
来源：http://sch.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hja.hysaishi.cn

[R52] 统计行数
来源：http://fuf.hammf.cn

wc -l a.txt
来源：http://fmx.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://axl.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vaz.sweek.top

[R54] 比较两个文件
来源：http://lwh.tianlin.xyz

diff a.txt b.txt
来源：http://oll.sxryk.cn

[R55] 压缩与解压
来源：http://sxh.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tjg.xuanzx.com

[R56] 远程拷贝
来源：http://dud.fengsongda.top

scp file user@host:/path/
来源：http://gnb.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://rpl.yuxming.cn

ssh user@host 'uptime'
来源：http://ztp.feifeiyinyue.top

[R58] 下载文件
来源：http://rll.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nyn.iojbl.cn

[R59] 发 POST JSON
来源：http://wca.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zgq.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://hnb.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jne.yvedp.cn

[R61] 磁盘占用
来源：http://boa.hfpthk.cn

df -h;  du -sh *
来源：http://ewr.vehdjk.com

[R62] 找最占空间的文件
来源：http://bvu.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://tzl.yangfankeji.com

[R63] 内存与进程
来源：http://pkk.cheryme.top

free -h;  ps aux | grep nginx
来源：http://znj.vqdsnc.cn

[R64] 结束进程
来源：http://lug.ppjwa.cn

kill -9 $(pgrep -f app.py)
来源：http://hwh.yuxming.cn

[R65] 查看端口占用
来源：http://agh.zhiwuduotai.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bxr.c1oappe.top

[R66] 定时任务
来源：http://cmu.birdmap.top

crontab -e;  crontab -l
来源：http://jad.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://kdk.yueranfly.top

openssl rand -hex 16
来源：http://qqv.chenzaomai.com

[R68] 计算文件校验值
来源：http://hym.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://boq.ppjwa.cn

[R69] 生成随机密码
来源：http://cgo.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://has.ppjwa.cn

[R70] 时间戳与互转
来源：http://qhb.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://gcd.pengpengdd.cyou

[R71] 日期格式化
来源：http://lex.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vcg.ydjk.org.cn

[R72] 等待端口就绪
来源：http://zfz.ydjk.org.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://orb.sjlbkw.cn

[R73] 分割大日志
来源：http://ram.xziqi.cn

split -l 1000 big.log part_
来源：http://ssp.meibo888.top

[R74] 批量重命名
来源：http://hgg.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lns.jqgfzy.top

[R75] 导出环境变量
来源：http://cgd.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://gls.cdnleiting.top

[R76] 使用临时文件
来源：http://auj.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pig.jlsjyb.cn

[R77] 读取用户输入
来源：http://hlr.sysykeji.top

read -rp "请输入: " ans
来源：http://fuw.fehbvm.com

[R78] 交互式菜单
来源：http://zkq.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hpy.bjfxy.top

[R79] 解析命令行选项
来源：http://gty.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gpo.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://aws.yonumen.top

time ./run.sh
来源：http://vgm.tarul.cn

================================================================================
来源：http://tmc.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://bka.zhixingplan.top

================================================================================
来源：http://sij.havefunace.top

[S01] C：Hello World
来源：http://fmm.nanxinkj.top

#include <stdio.h>
来源：http://wyq.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://wta.epnwcf.com

[S02] C：变量与格式化输出
来源：http://txw.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://xhw.pycfn.com

[S03] C：读入整数
来源：http://loi.xinyue.icu

int x; scanf("%d", &x);
来源：http://qlc.hnxiangtu.top

[S04] C：字符串复制
来源：http://ebl.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bhl.zdbjq.cn

[S05] C：字符串长度
来源：http://cgy.guowangkeji.top

strlen(s)
来源：http://iyb.svipenyu.cn

[S06] C：字符串比较
来源：http://cjd.zdbjq.cn

strcmp(a, b) == 0
来源：http://udu.tianlin.xyz

[S07] C：数组遍历求和
来源：http://rla.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://isw.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://dfn.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://txh.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://cqa.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://izn.ydzc1.top

[S10] C：指针与解引用
来源：http://kfs.ybcxt.top

int *p = &a;  *p = 5;
来源：http://ddp.snrcjt.cn

[S11] C：逐行读文件
来源：http://jfd.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://ijv.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://evk.sufxvd.cn

fclose(f);
来源：http://fng.zhengqikj.top

[S12] C：写文件
来源：http://joh.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cfr.cucudq.cn

[S13] C：宏定义
来源：http://fkd.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jpr.9152youxi.cn

[S14] C：枚举
来源：http://qer.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://sxy.zhixingplan.top

[S15] C：类型转换
来源：http://vnt.cucudq.cn

(double) a / b
来源：http://zqf.ppjwa.cn

[S16] C：位操作置位
来源：http://khi.uphjek.com

x |= (1 << 3);
来源：http://ctz.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://swb.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ldx.nwbrower.top

[S18] C：命令行参数
来源：http://lty.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://mmu.haohaochexian.top

[S19] C：快速排序
来源：http://ahu.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://mic.c1oappe.top

[S20] C：二分查找
来源：http://ldt.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nsf.zdqjudy.top

[S21] C：字符类别判断
来源：http://hfr.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qey.xylfe.cn

[S22] C：字符串转数字
来源：http://osb.9152youxi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cdt.52xcode.cn

[S23] C：随机数
来源：http://eln.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://knr.chenzaomai.com

[S24] C：获取本地时间
来源：http://kvo.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hhl.sxryk.cn

[S25] C：内存拷贝
来源：http://atp.yueranfly.top

memcpy(dst, src, n);
来源：http://bhh.yanxiufei.cn

[S26] C：内存清零
来源：http://xsm.sysykeji.top

memset(a, 0, sizeof a);
来源：http://lvg.gogol.net.cn

[S27] C：定义常量
来源：http://umd.hongshengwenyu.top

const double PI = 3.14159;
来源：http://nah.iojbl.cn

[S28] C：静态变量
来源：http://ved.birdmap.top

static int counter = 0;
来源：http://qlu.yonumen.top

[S29] C：变参函数
来源：http://pps.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kyf.tian-w.cn

[S30] C：头文件保护
来源：http://qkj.cucudq.cn


<!-- 参考信息 -->