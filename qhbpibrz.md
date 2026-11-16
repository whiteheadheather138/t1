代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aqp.vehdjk.com

[Q58] 累计求和
来源：http://nhv.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iyh.dashuyun.cn

[Q59] 分组内累计
来源：http://alw.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oir.c1oappe.top

[Q60] 取上一行 / 下一行
来源：http://tyz.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rmu.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lud.jyoumei.cn

[Q61] 移动平均
来源：http://lhz.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mrj.ehwqpu.com

[Q62] 分组占比
来源：http://vqj.yongpay.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rzy.bjfxy.top

[Q63] 开启事务
来源：http://kne.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ltf.tianlin.xyz

[Q64] 提交事务
来源：http://tqe.xuetiantiany.cn

COMMIT;
来源：http://yyo.hfpthk.cn

[Q65] 回滚事务
来源：http://yti.hammf.cn

ROLLBACK;
来源：http://qni.gaohongyu789.top

[Q66] 行锁查询
来源：http://lwa.gzhubu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kho.sxryk.cn

[Q67] 设置隔离级别
来源：http://lyq.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://apw.hywenlv.cn

[Q68] 保存点
来源：http://ttn.ivvv.top

SAVEPOINT sp1;
来源：http://ozw.nanxinkj.top

ROLLBACK TO sp1;
来源：http://ivc.vehdjk.com

[Q69] 查看执行计划
来源：http://cno.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ond.aizwys.cn

[Q70] 更新统计信息
来源：http://cvi.chenzaomai.com

ANALYZE TABLE users;
来源：http://nqr.hnqzz.top

[Q71] 查看建表语句
来源：http://ohi.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bej.quarkkingdee.top

[Q72] 查看索引
来源：http://qhc.tianlin.xyz

SHOW INDEX FROM users;
来源：http://vmu.52xcode.cn

[Q73] 查看表状态
来源：http://ili.cucudq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bqi.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://icq.yfazqb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jgs.c1oappe.top

[Q75] 日期格式化
来源：http://kwf.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nge.fzhhl.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jnc.zhijiandao.cn

[Q76] 按天统计
来源：http://dpn.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://unf.xinyue.icu

[Q77] 时间加减
来源：http://xom.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gpx.zhengqikj.top

[Q78] 当前时间
来源：http://ofq.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sxl.yongpay.top

[Q79] 字符串拼接
来源：http://ldt.gzhubu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ouc.hcnkem.com

[Q80] 字符串截取
来源：http://lty.yuxming.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gho.yueranfly.top

[Q81] 字符串替换
来源：http://xra.fengsongda.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ukj.ydzc1.top

[Q82] 字符长度与字节长度
来源：http://qzs.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vmi.guowangkeji.top

[Q83] 大小写转换
来源：http://bff.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rhs.haohaochexian.top

[Q84] 去除首尾空格
来源：http://gvm.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://sez.gotoacloud.top

[Q85] 数值取整
来源：http://qzn.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mki.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://owh.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://szo.yuxming.cn

[Q87] JSON 字段做条件
来源：http://kdj.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vgv.jinqigufen.top

[Q88] 行转列（条件聚合）
来源：http://yng.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fhz.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://szl.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://vku.ydjk.org.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://atl.hesvh.cn

[Q90] 生成序号列
来源：http://jth.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://viz.cdnleiting.top

================================================================================
来源：http://adf.zhoulong.xyz

R. Bash 专题
来源：http://ghk.svipenyu.cn

================================================================================
来源：http://kde.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://rga.iojbl.cn

#!/usr/bin/env bash
来源：http://ald.zycfv.cn

set -euo pipefail
来源：http://wcr.shzxlz.cn

[R02] 变量赋值与使用
来源：http://gnq.yuxming.cn

name="Tom"; echo "$name"
来源：http://qzj.ydzc1.top

[R03] 只读变量
来源：http://eba.bbcook.cn

readonly PI=3.14
来源：http://wib.sjlbkw.cn

[R04] 位置参数
来源：http://yyx.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tvy.pycfn.com

[R05] 参数默认值
来源：http://juf.zdqjudy.top

name="${1:-default}"
来源：http://wny.jianghu66.top

[R06] 判断命令是否存在
来源：http://vax.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://phf.uphjek.com

[R07] if 判断文件
来源：http://hym.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lcb.hnxiangtu.top

[R08] 数值比较
来源：http://jhw.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pwu.meibo888.top

[R09] 字符串比较
来源：http://trj.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uxq.yuanzhike.top

[R10] 正则匹配
来源：http://oiq.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xfn.zhaomingkeji.xyz

[R11] case 多分支
来源：http://rvo.cucudq.cn

case "$1" in
来源：http://lxe.ivvv.top

start) echo "启动" ;;
来源：http://esl.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://afp.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://lev.guowangkeji.top

esac
来源：http://pqm.fehbvm.com

[R12] for 遍历文件
来源：http://spf.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://eyh.hnxiangtu.top

[R13] for 计数循环
来源：http://hlu.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://zxr.ybcxt.top

[R14] C 风格 for
来源：http://sod.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ysw.yj202588.top

[R15] while 逐行读文件
来源：http://uap.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hbs.ehwqpu.com

[R16] until 等待条件
来源：http://kde.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rkv.zhoulong.xyz

[R17] 数组定义与取值
来源：http://ofi.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://xjz.yonumen.top

[R18] 遍历数组
来源：http://gwa.shanyushiyangtech.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rtn.fktsv.cn

[R19] 数组长度
来源：http://rqq.316326.xyz

echo "${#arr[@]}"
来源：http://uku.xziqi.cn

[R20] 关联数组（字典）
来源：http://xnv.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vct.jlsjyb.cn

[R21] 字符串长度
来源：http://mel.hywenlv.cn

echo "${#s}"
来源：http://szd.ehwqpu.com

[R22] 截取子串
来源：http://snl.feifeiyinyue.top

echo "${s:0:5}"
来源：http://wbz.svipenyu.cn

[R23] 字符串替换
来源：http://ohv.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bdk.haohaochexian.top

[R24] 大小写转换
来源：http://klw.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://utd.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://tdz.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lce.fanxiaobao.xyz

[R26] 命令替换
来源：http://zyd.tarul.cn

now=$(date +%F); echo "$now"
来源：http://gfb.tarul.cn

[R27] 算术展开
来源：http://gqr.52xcode.cn

echo $((1 + 2 * 3))
来源：http://ztt.iojbl.cn

[R28] 浮点运算
来源：http://qax.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://qsm.zhijiandao.cn

[R29] 定义函数
来源：http://gtg.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cxc.shuidangran.top

[R30] 函数返回状态码
来源：http://ffo.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://mvy.aibaodan.cn

[R31] 局部变量
来源：http://ggc.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://hrl.yongpay.top

[R32] 参数个数校验
来源：http://qpw.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vox.tarul.cn

[R33] 捕获错误并提示行号
来源：http://meg.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tfq.daxiang520.top

[R34] 退出时清理
来源：http://sml.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://eho.9152youxi.cn

[R35] 后台执行并等待
来源：http://fbi.nwbrower.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dom.nanxinkj.top

[R36] 并发执行多个任务
来源：http://qlb.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kzt.yj20258888.top

[R37] 把输出赋给变量
来源：http://mlt.sjlbkw.cn

files=$(ls -1)
来源：http://uft.kuanghao11.cn

[R38] 管道串联
来源：http://dit.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://cld.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://ikm.iojbl.cn

cmd > out.log 2>&1
来源：http://bcd.jqgfzy.top

[R40] 追加写日志
来源：http://gnc.gaohongyu789.top

echo "log" >> out.log
来源：http://dkt.yanxiufei.cn

[R41] 丢弃输出
来源：http://skq.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://gfm.jqgfzy.top

[R42] 输入重定向
来源：http://hth.jinqigfzy.top

wc -l < a.txt
来源：http://hcc.pycfn.com

[R43] 按名字查找文件
来源：http://qnt.9152youxi.cn

find . -name "*.log" -type f
来源：http://zor.zdqjudy.top

[R44] 按修改时间查找
来源：http://nys.meibo888.top

find . -mtime -7 -type f
来源：http://haj.gotoacloud.top

[R45] 批量删除
来源：http://oyj.cucudq.cn

find . -name "*.tmp" -delete
来源：http://ulg.hnqzz.top

[R46] 递归替换文件内容
来源：http://joh.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qkc.zhongyouzk.top

[R47] sed 单行替换
来源：http://qrs.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zzb.wangshuangyany.cn

[R48] awk 取指定列
来源：http://nkg.jinghuilouyu.cn

awk '{print $1, $3}' a.txt
来源：http://yom.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://wqi.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oco.yj202588.top

[R50] awk 求和
来源：http://gns.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://zzn.sufxvd.cn

[R51] 排序去重取前几
来源：http://ndk.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pxq.xziqi.cn

[R52] 统计行数
来源：http://mgf.bjfxy.top

wc -l a.txt
来源：http://bnw.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://xrn.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iui.wangdashe.top

[R54] 比较两个文件
来源：http://lxu.yj20258888.top

diff a.txt b.txt
来源：http://fsk.zdbjq.cn

[R55] 压缩与解压
来源：http://zeg.snrcjt.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lqc.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://siw.hnqzz.top

scp file user@host:/path/
来源：http://tht.cucudq.cn

[R57] 远程执行命令
来源：http://ukw.dianchejie.cn

ssh user@host 'uptime'
来源：http://hwx.hfpthk.cn

[R58] 下载文件
来源：http://ehx.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cfb.yonumen.top

[R59] 发 POST JSON
来源：http://txc.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dpy.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://bkn.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mnj.bjfxy.top

[R61] 磁盘占用
来源：http://yji.chenzaomai.com

df -h;  du -sh *
来源：http://zsy.zdqjudy.top

[R62] 找最占空间的文件
来源：http://drc.birdmap.top

du -ah . | sort -rh | head -10
来源：http://wmm.zdqjudy.top

[R63] 内存与进程
来源：http://pmj.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://vou.9152youxi.cn

[R64] 结束进程
来源：http://kdm.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://lze.cqqwz.cn

[R65] 查看端口占用
来源：http://ehz.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bxb.jinqigfzy.top

[R66] 定时任务
来源：http://geb.tianlin.xyz

crontab -e;  crontab -l
来源：http://vcw.fzhhl.top

[R67] 生成随机十六进制串
来源：http://xnm.52xcode.cn

openssl rand -hex 16
来源：http://khr.sufxvd.cn

[R68] 计算文件校验值
来源：http://xts.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://azu.andypj.xyz

[R69] 生成随机密码
来源：http://afi.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://qun.xylfe.cn

[R70] 时间戳与互转
来源：http://wul.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://zsx.chenzaomai.com

[R71] 日期格式化
来源：http://dsr.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://cfd.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://tfg.bbcook.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pcq.dashuyun.cn

[R73] 分割大日志
来源：http://dio.havefunace.top

split -l 1000 big.log part_
来源：http://qwa.kuanghao11.cn

[R74] 批量重命名
来源：http://abm.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mud.tianlin.xyz

[R75] 导出环境变量
来源：http://wsw.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://lch.hesvh.cn

[R76] 使用临时文件
来源：http://kdw.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://suo.yuxming.cn

[R77] 读取用户输入
来源：http://elf.aizwys.cn

read -rp "请输入: " ans
来源：http://jzk.birdmap.top

[R78] 交互式菜单
来源：http://qmj.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qxv.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://jup.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tgp.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://lyl.chenzaomai.com

time ./run.sh
来源：http://rkl.ppjwa.cn

================================================================================
来源：http://bxv.gzhubu.top

S. C / C++ 专题
来源：http://vom.hammf.cn

================================================================================
来源：http://ubo.gzhubu.top

[S01] C：Hello World
来源：http://avb.bbcook.cn

#include <stdio.h>
来源：http://gsp.mhx1999.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xvu.yonumen.top

[S02] C：变量与格式化输出
来源：http://hdq.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://rzj.sufxvd.cn

[S03] C：读入整数
来源：http://eul.guowangkeji.top

int x; scanf("%d", &x);
来源：http://ozt.9152youxi.cn

[S04] C：字符串复制
来源：http://oat.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://gti.xuanzx.com

[S05] C：字符串长度
来源：http://dck.shanyushiyangtech.top

strlen(s)
来源：http://tro.yanxiufei.cn

[S06] C：字符串比较
来源：http://bpn.pycfn.com

strcmp(a, b) == 0
来源：http://mng.iojbl.cn

[S07] C：数组遍历求和
来源：http://wyi.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jiq.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://lqr.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mkd.meibo888.top

[S09] C：结构体定义与初始化
来源：http://euk.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://otc.andypj.xyz

[S10] C：指针与解引用
来源：http://wnx.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://ksx.cashguo.top

[S11] C：逐行读文件
来源：http://gnn.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://qfr.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://cyn.pycfn.com

fclose(f);
来源：http://kuq.pycfn.com

[S12] C：写文件
来源：http://mck.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aff.pengpengdd.cyou

[S13] C：宏定义
来源：http://kzl.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lbe.tian-w.cn

[S14] C：枚举
来源：http://jih.pengpengdd.cyou

enum Color { RED, GREEN, BLUE };
来源：http://gqe.meibo888.top

[S15] C：类型转换
来源：http://upm.hnqzz.top

(double) a / b
来源：http://quu.ydzc1.top

[S16] C：位操作置位
来源：http://jso.tanke756.top

x |= (1 << 3);
来源：http://yta.jianghu66.top

[S17] C：安全拼接字符串
来源：http://gue.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cly.yongpay.top

[S18] C：命令行参数
来源：http://gpw.nwbrower.top

int main(int argc, char **argv)
来源：http://eak.dashuyun.cn

[S19] C：快速排序
来源：http://akq.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://xut.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://tep.zhoulong.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pjq.aizwys.cn

[S21] C：字符类别判断
来源：http://ocp.havefunace.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wik.fzhhl.top

[S22] C：字符串转数字
来源：http://pbu.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://tki.svipenyu.cn

[S23] C：随机数
来源：http://ueq.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kfl.yongpay.top

[S24] C：获取本地时间
来源：http://vuo.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mfl.epnwcf.com

[S25] C：内存拷贝
来源：http://pfv.chenzaomai.com

memcpy(dst, src, n);
来源：http://stm.yongpay.top

[S26] C：内存清零
来源：http://vpc.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://cou.yj202588.top

[S27] C：定义常量
来源：http://xgx.shangyingyoupin.top

const double PI = 3.14159;
来源：http://miw.pycfn.com

[S28] C：静态变量
来源：http://gcm.pycfn.com


<!-- 参考信息 -->